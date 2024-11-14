---
layout: note
title: "Diccionario en C++"
author: Jesús Peralta
date: 2022-01-06
tags: programacion
---

Código en GitHub: [https://github.com/zettafounder/diccionario-cpp/blob/main/diccionario.cpp](https://github.com/zettafounder/diccionario-cpp/blob/main/diccionario.cpp)

## Código

~~~cpp
#include<stdio.h>
#include<string.h>
#include<stdlib.h>
int main(){
    char palabra[5][25];
    char significado[5][25];
    char bpalabra[25];
    char mpalabra[25];
    char epalabra[25];
    int o, j, salvarj=-1, salvari, ni=0;
    
    do{
        system("cls");
        printf("Menu---\n");
        printf("1. Agregar palabra\n");
        printf("2. Mostrar palabras\n");
        printf("3. Buscar palabra\n");
        printf("4. Modificar palabra\n");
        printf("5. Eliminar palabra\n");
        printf("Seleccion: ");
        scanf("%d",&o);
        system("cls");

        switch(o){
            case 1:
                j=salvarj;
                j=j+1;
                ni=ni+1;
                printf("Agregar palabra---\n\n");
                printf("Introduzca palabra: ");
                scanf("%s",palabra[j]);
                printf("Introduzca significado: ");
                scanf("%s",significado[j]);
                salvarj=j;
                break;
            case 2:
                printf("Todas las palabras\n\n");
                for(j=0;j<ni;j++){
                    printf("Palabra: %s\n",palabra[j]);
                    printf("Significado: %s\n\n",significado[j]);
                }
                getchar();
                break;
            case 3:
                printf("Buscar palabra---\n\n");
                printf("Introduzca la palabra: ");
                scanf("%s",bpalabra);
                for(j=0;j<ni;j++){
                    if((strcmp(palabra[j],bpalabra))==0){
                        printf("Palabra: %s\n",palabra[j]);
                        printf("Significado: %s\n",significado[j]);
                        getchar();
                    }
                }
                break;
            case 4:
                printf("Modificar palabra\n\n");
                printf("Introduzca la palabra: ");
                scanf("%s",mpalabra);
                for(j=0;j<ni;j++){
                    if((strcmp(palabra[j],mpalabra))==0){
                        printf("Introduzca nuevo significado: ");
                        scanf("%s",significado[j]);
                    }
                }
                break;
            case 5:
                printf("Eliminar palabra---\n\n");
                printf("Introduzca palabra: ");
                scanf("%s",epalabra);
                for(j=0;j<ni;j++){
                    if((strcmp(palabra[j],epalabra))==0){
                        salvari=j;
                        for(j=salvari;j<ni;j++){
                            strcpy(palabra[j],palabra[j+1]);
                            strcpy(significado[j],significado[j+1]);
                        }
                        ni=ni-1;
                        salvarj=j-2;
                    }
                }
                break;
        }getchar();
    }while(1);

    getchar();
    return 0;
}
~~~