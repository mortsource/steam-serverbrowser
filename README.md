# Server Browser+ for Steam

<p align="center">
  <a href="#enhanced-browsing">Enhanced Browsing</a> &nbsp;&bull;&nbsp;
  <a href="#spam-filtering">Spam Filtering</a> &nbsp;&bull;&nbsp;
  <a href="#install">Install</a>
</p>
<p align="center">
    <img alt="GitHub Release" src="https://img.shields.io/github/v/release/mortsource/steam-serverbrowser">
    <img alt="GitHub Downloads (all assets, all releases)" src="https://img.shields.io/github/downloads/mortsource/steam-serverbrowser/total">
</p>

Server Browser+ is a plugin for the native Steam game server browser. This project requires [Millennium aka SteamBrew](https://steambrew.app), a framework for Steam. It is used commonly for themes but also plugins, install is quick and simple. Report any issues or suggest improvements, this is in active development.

## Enhanced Browsing 
![image](./docs/readme_enhanced.PNG)  

Splits the native browser into two panes: a virtualized server list with images and a live Leaflet map, synced together. Servers are clustered by region and expand when zoomed. Filters and context menus behave as expected. Quick access tabs for popular games and removed dead games.

## Spam Filtering
<p align="center">
    <img alt="CS" src="https://img.shields.io/badge/counter_strike-enabled-brightgreen?style=for-he-badge">
    <img alt="CSS" src="https://img.shields.io/badge/cs_source-enabled-brightgreen?style=for-he-badge">
    <img alt="CSGO" src="https://img.shields.io/badge/cs_go-enabled-brightgreen?style=for-he-badge">
</p>

![image](./docs/readme_filtering.PNG)  

Individually toggleable filters made to catch different types of master server abuse within the Counter-Strike franchise. Filters sit between the callback to the server browser and add virtually zero overhead by using compiled RegEx patterns, subnet masks and GeoLite MMDB.

| Filter | Example |
|---|---|
| **MASTER BLOCKLIST*** | `*.*.*.*/16, /sgaming.ru/i` |
| **CYRILLIC** | `спам-сервер` |
| **EMOJIS** | `🏆🏆🏆` |
| **PLAYER SPOOFING** | `255/255` |  

*Acquired automatically on startup or on-demand in settings

## Install
> [!WARNING]
> If you used the beta of this project, **pureBrowser**, make sure to delete it from your plugins to ensure it doesn't conflict

1. Go to [Millennium (SteamBrew)](https://steambrew.app), download and install.
<img src="./docs/readme_install1.png" width="500" style="padding-bottom: 30px">  

2. Download the latest [release](https://github.com/mortsource/discord-gemini/releases) of the plugin, currently it is ![GitHub Release](https://img.shields.io/github/v/release/mortsource/steam-serverbrowser). Extract the ZIP and paste the contents into your Steam installation likely at ```C:\Program Files (x86)\Steam```.
<img src="./docs/readme_install2.png" width="500" style="padding-bottom: 30px">

3. Restart Steam and go to Steam > Millennium in the top bar. Navigate to the 'Plugins' section and enable 'ServerBrowserPlus'. You will be prompted to restart again.
<img src="./docs/readme_install3.png" width="500">

*Slava Ukraini* 🇺🇦