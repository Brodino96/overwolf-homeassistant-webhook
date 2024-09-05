# overwolf-homeassistant-webhook

Send game events from overwolf to Home Assistant.

## Disclaimer

This project is not endorsed by or affiliated with Overwolf or Home Assistant.

## Setup

A [step by step setup guide](https://github.com/lociii/homeassistant-overwolf-status/blob/main/info.md) has been added on the [Home Assistant integration repository](https://github.com/lociii/homeassistant-overwolf-status).

## Helpers

### Scrape game features

Overwolf is an ever expanding and improving ecosystem. From time to time they add support for new games or new info/events in existing games.
To make it easier for this app to stay up to date, a scraper has been implemented to export an updates list of `interestingFeatures` to be used in `src/consts.ts`.

Just run the VSCode task `Scrape game features`, copy them and paste to the `src/consts.ts`.

Then copy the list of game IDs and put the new values in all the relevant fields of `public/manifest.json`

## How to contribute

### VSCode setup

-   Install Docker Desktop for Windows
-   Install VSCode
-   Open VSCode
-   Install the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension
-   Open the project in the remote container
-   You need to run either `npm install` or the VSCode task `Install dependencies` to install the dependencies

### Build the application

-   Run the VSCode task `Build` (`CTRL + Shift + B` or `CMD + Shift + B` by default)

### Test it

Load the application as an unpackaged app in Overwolf:

-   Open Overwolf
-   Open Settings
-   Open the `About` tab
-   Click on `Development options`
-   Click `Load unpacked extension...`
-   Select the `dist` folder.

PS: There is little to no reason to try and run the app, if you're not whitelisted by Overwolf, the app will not work. They block it at some base level. So unless you actively have developed on Overwolf before, you will not be able to test the app.

## Contributors

In order of first contribution date

-   [Arco "Tex" Dielhof](https://github.com/Arco-Dielhof)
-   [Jens "loci" Nistler](https://github.com/lociii)
