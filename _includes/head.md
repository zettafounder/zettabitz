<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  {%- seo -%}
  <link rel="stylesheet" href="{{ "/assets/css/style.css" | relative_url }}">
  {%- feed_meta -%}
  {%- if jekyll.environment == 'production' and site.google_analytics -%}
    {%- include google-analytics.html -%}
  {%- endif -%}

  {%- include custom-head.html -%}
  
  <style>
        .PageNavigation {
        font-size: 14px;
        display: block;
        width: auto;
        overflow: hidden;
        }

        .PageNavigation a {
        display: block;
        width: 50%;
        float: left;
        margin: 1em 0;
        }

        .PageNavigation .next {
        text-align: right;
        }
  </style>
  
</head>