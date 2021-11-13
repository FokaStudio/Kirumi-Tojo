### Table of Contents
- [Contributing](#contributing)
- [Copyright Notice](#copyright-notice)
- [Code Conventions](#code-conventions)
- [Addons](#addons)

# Contributing
![Lines of code](https://img.shields.io/tokei/lines/github/FokaStudio/Kirumi-Tojo?color=1&label=Lines%20of%20code&logo=Visual%20Studio%20Code&logoColor=blue&style=for-the-badge)
[![License](https://img.shields.io/badge/License-FSVODWTFYWWT-orange?style=for-the-badge&logo=github)](LICENSE.md)

As I have stated in [README.md](README.md), I use *Skript* paired with for everything related to coding in there, so you have to use this too!

# Copyright Notice
[![License](https://img.shields.io/badge/License-FSVODWTFYWWT-orange?style=for-the-badge&logo=github)](LICENSE.md)

This repo and all work inside it is licensed under [**FokaStudio's Very Own DO WHATEVER THE FUCK YOU WANT WITH THIS License**](LICENSE.md), meaning that:
1. You are free to download the work created here and use it for yourself *(on both private and public servers)*
2. You must not remove the copyright and ownership notices 
3. You can redistribute the work if you are sticking to certain conditions
4. You must __show me__ the modifications you made **if asked by me**
5. If you are contributing - you have to license your work under the same license and put this on top of the file:
   
    ```t
    #
    # Copyright © FokaStudio 2020-2021 
    # Contributed to Tojo-san Bot by <contributors>
    #
    # https://github.com/FokaStudio/Kirumi-Tojo (this line is optional)
    #                                           (followed with this line)
    ```
   Replace `<contributors>` with names/usernames/whatever of all people who have put some effort in making of the code.

6. Any script made for the bot must be free. Contents of this repo will always be accesible to everyone (unless Foka takes their rights away)

# Code Conventions
1. All work must be properly commented for purpose of letting everyone who is reviewing a pull request know what a particular part of the script is doing
   1. Comments can be added after the initial PR with the contributed material
   2. Commenting:
        ```
        # single hastag - least important stuff
        #! hastag and exclamation mark - important stuff
        #!! hastag and 2 exclamation marks - additional info
        ```
        Follow this format, because of VSC's formatting of comments

2. If you wish to use **skript-reflect** make sure that:
   1. You follow [*skript-reflect's code conventions*](https://tpgamesnl.gitbook.io/skript-reflect/code-conventions)
        - We aren't so strict when it comes to convention #1, but we do when it comes to convention #2 and #4
   2. Don't overuse reflections, e.g. if have to use `event.getBlock()` several times, make it more like this:
        ```applescript
        set {_block_} to event.getBlock()
        {_block_}.doStuff1()
        {_block_}.doMoreStuff1()
        {_block_}.doEvenMoreStuff1()
        ```
        ***Too many reflections lag terribly and slow parse time. Do it like this if you want to use many of the same reflections***
    3. Don't use reflections for something that is possible with vanilla Skript or any of the Addons! Better read [documentation](https://skripthub.net/docs/) first! More on that in [#addons](#addons)!

# Addons
We use several addons to Skript to make our Scripts work. Here is a list with their purposes:

   - **SkQuery** - `AND()` and `OR()` functions, since *SkJade* has a slow parse time with those, branching and some other non-minecraft related features
   - **DiSky** - *wel duh...*
   - **MorkazSK** - sorting of Leaderboard
   - **Skent** - file manipulation
   - **SkImage** - EXP Cards and such
   - **skript-reflect** - calling Java static methods inside Skript
   - **skript-logs** - *not used yet*
   - **skript-db** - MySQL
   - **Reqn** - web requests
   - **SkriptJSON** - mapping bodies of web requests to variables
   - **skript-yaml** - YAML databases
   