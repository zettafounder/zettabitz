---
layout: index
---

YouTube:  <a href="https://youtube.com/%40ZettaBitz" target="_blank">**Zetta Bitz**</a>.<br>**GNU/Linux**,  **Bitcoin**,  **Android libre**, **Privacidad**.

---
<br>
## Software

OS: <a href="https://endeavouros.com" target="_blank">**EndeavourOS**</a>, <a href="https://www.debian.org" target="_blank">**Debian**</a>, <a href="https://pop.system76.com" target="_blank">**Pop! OS**</a>, <a href="https://tails.boum.org" target="_blank">**Tails**</a>.<br>
Android: <a href="https://lineageos.org" target="_blank">**LineageOS**</a>.<br>
Mensajería: <a href="https://signal.org" target="_blank">**Signal**</a>, <a href="https://getsession.org" target="_blank">**Session**</a>, <a href="https://simplex.chat" target="_blank">**SimpleX**</a>, <a href="https://briarproject.org" target="_blank">**Briar**</a>, <a href="https://cwtch.im" target="_blank">**Cwtch**</a>, <a href="https://telegram.org" target="_blank">**Telegram**</a>, <a href="https://wire.com" target="_blank">**Wire**</a>, <a href="https://threema.ch" target="_blank">**Threema**</a>, <a href="https://keybase.io" target="_blank">**Keybase**</a>, <a href="https://element.io" target="_blank">**Element**</a>, <a href="https://conversations.im" target="_blank">**Conversations**</a>.<br>
Nube: <a href="https://proton.me" target="_blank">**Proton Drive**</a>.<br>
Navegador: <a href="https://www.mozilla.org" target="_blank">**Firefox**</a>, <a href="https://www.torproject.org" target="_blank">**Tor Browser**</a>.<br>
Buscador: <a href="https://duckduckgo.com" target="_blank">**DuckDuckGo**</a>.<br>
Bitcoin Wallets: <a href="https://electrum.org" target="_blank">**Electrum**</a>, <a href="https://blockstream.com/green" target="_blank">**Green**</a>, <a href="https://bluewallet.io" target="_blank">**BlueWallet**</a>, <a href="https://phoenix.acinq.co" target="_blank">**Phoenix**</a>, <a href="https://www.walletofsatoshi.com" target="_blank">**WalletOfSatoshi**</a>.<br>
Email: <a href="https://proton.me" target="_blank">**Proton Mail**</a>, <a href="https://www.thunderbird.net" target="_blank">**Thunderbird**</a>.<br>
VPN: <a href="https://proton.me" target="_blank">**Proton VPN**</a>.<br>
Nostr: <a href="https://www.yakihonne.com/yakihonne-mobile-app" target="_blank">**YakiHonne**</a>.<br>
Contraseñas: <a href="https://proton.me" target="_blank">**Proton Pass**</a>, <a href="https://keepass.info/download.html" target="_blank">**KeePass**</a>.<br>
2FA: <a href="https://getaegis.app" target="_blank">**Aegis**</a>.<br>
Criptografia: <a href="https://apps.kde.org/es/kleopatra/" target="_blank">**Kleopatra**</a>, <a href="https://www.openkeychain.org" target="_blank">**OpenKeychain**</a>, <a href="https://paranoiaworks.mobi/sse/" target="_blank">**Secret Space Encryptor**</a>.<br>
Notas: <a href="https://keep.google.com" target="_blank">**Keep**</a>, <a href="https://github.com/OmGodse/Notally" target="_blank">**Notally**</a>.<br>
Tareas y calendario: <a href="https://taskito.io" target="_blank">**Taskito**</a>.<br>Marcadores: <a href="https://raindrop.io" target="_blank">**Raindrop**</a>.<br>Podcast: <a href="https://fountain.fm" target="_blank">**Fountain**</a>, <a href="https://antennapod.org" target="_blank">**AntennaPod**</a>.<br>Otros: <a href="https://www.aimp.ru" target="_blank">**AIMP**</a>, <a href="https://github.com/spacecowboy/feeder" target="_blank">**Feeder**</a>, <a href="https://organicmaps.app" target="_blank">**Organic Maps**</a>, <a href="https://play.google.com/store/apps/details?id=com.cxinventor.file.explorer" target="_blank">**Cx File Explorer**</a>, <a href="https://f-droid.org" target="_blank">**F-Droid**</a>, <a href="https://www.deepl.com" target="_blank">**DeepL**</a>, <a href="https://newpipe.net" target="_blank">**NewPipe**</a>, <a href="https://disroot.org" target="_blank">**Disroot**</a>.

---
<br>

## Te puede interesar

&raquo; [**Crear USB booteable de linux usando el comando dd**](https://zettafounder.github.io/zettabitz/notes/2024-04-17-comando-dd.html)<br>&raquo; [**Elimina el bloatware de tu android con adb shell**](https://zettafounder.github.io/zettabitz/notes/2022-01-07-eliminar-apps-preinstaladas-android.html)

---
<br>

## Últimos posts del blog

{% for post in site.posts  | limit: 3 %}
  <div>{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    <time class="dt-published" datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">
      {{ post.date | date: date_format }}
    </time>
    {%- if post.modified_date -%}
      ~ 
      {%- assign mdate = post.modified_date | date_to_xmlschema -%}
      <time class="dt-modified" datetime="{{ mdate }}" itemprop="dateModified">
        {{ mdate | date: date_format }}
      </time>
    {%- endif -%} - <a href=".{{ post.url }}"><strong>{{ post.title }}</strong></a></div> 
{% endfor %}