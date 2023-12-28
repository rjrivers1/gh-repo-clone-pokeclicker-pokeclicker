[![GitHub package.json version (branch)](https://img.shields.io/github/package-json/v/pokeclicker/pokeclicker/develop?label=dev%20version)](https://github.com/pokeclicker/pokeclicker/tree/develop)<br/>
[![GitHub package.json version (branch)](https://img.shields.io/github/package-json/v/pokeclicker/pokeclicker/master?label=live%20version)](https://www.pokeclicker.com/)<br/>
[![Build Status](https://img.shields.io/travis/com/pokeclicker/pokeclicker?logo=travis)](https://travis-ci.com/pokeclicker/pokeclicker)<br/>
[![Discord](https://img.shields.io/discord/450412847017754644?color=7289DA&label=Discord&logo=discord)](https://discord.gg/a6DFe4p)

# PokéClicker
A game about catching Pokémon, defeating gym leaders, and watching numbers get bigger.

NOTE: PokéClicker is still in development!

You can try out the current state at https://www.pokeclicker.com/

You can reach out on discord to discuss your ideas and how to implement them: https://discord.gg/a6DFe4p

# Developer instructions

## Rules
- Make sure the build script is a success. We won't test PRs that fail the building script.
- We won't accept balance PRs, unless it's from a developer or Code Contributor (discord roles).
- Don't submit any changes within the `/docs` folder.
- PRs adding new translatable content should link to a PR in the [translation repo](https://github.com/pokeclicker/pokeclicker-translations) adding your new strings. See the Developer instructions on that repo for more info.

## Editor/IDE setup

We have an [EditorConfig](https://editorconfig.org/) and linting configured, to help everyone write similar code. You will find our recommended plugins for VSCode below, however you should be able to find a plugin for other IDEs as well.

* [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

## Building from Source

First make sure you have git and npm available as command-line utilities (so you should install Git and NodeJS if you don't have them already).

Open a command line interface in the directory that contains this README file, and use the following command to install PokéClicker's other dependencies locally:
```cmd
npm run clean
```

Then finally, run the following command in the command line interface to start a browser running PokéClicker.
```cmd
npm start
```

Changes to the sourcecode will automatically cause the browser to refresh.
This means you don't need to compile TypeScript yourself. Gulp will do this for you :thumbsup:


## Use Google cloud shell _(alternative)_
[![Google Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.png)](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/pokeclicker/pokeclicker&git_branch=develop&page=editor&open_in_editor=README.md)
```cmd
npm clean-install
npm start
```
Click the [Web Preview](https://cloud.google.com/shell/docs/using-web-preview) Button and select port `3001` from the displayed menu.
Cloud Shell opens the preview URL on its proxy service in a new browser window.

## Deploying a new version to Github Pages
Before deploying, check that the game compiles and starts up without errors. Then run:
```cmd
npm run website
```

After this command completes, push the changed files in the 'docs' directory to Github.



> Open this page at [https://rjrivers1.github.io/gh-repo-clone-pokeclicker-pokeclicker/](https://rjrivers1.github.io/gh-repo-clone-pokeclicker-pokeclicker/)

## Use as Extension

This repository can be added as an **extension** in MakeCode.

* open [https://makecode.microbit.org/](https://makecode.microbit.org/)
* click on **New Project**
* click on **Extensions** under the gearwheel menu
* search for **https://github.com/rjrivers1/gh-repo-clone-pokeclicker-pokeclicker** and import

## Edit this project

To edit this repository in MakeCode.

* open [https://makecode.microbit.org/](https://makecode.microbit.org/)
* click on **Import** then click on **Import URL**
* paste **https://github.com/rjrivers1/gh-repo-clone-pokeclicker-pokeclicker** and click import

#### Metadata (used for search, rendering)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
