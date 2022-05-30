# steamBackups

Visual console scipt using whiptail for backup/recovery games from steam.

On linux, steam archive tool uses only one thread, opens up annoing window which is completely blocking steam and backup multiple games into one archive.
And what if you want to update only one of these games ?

This script resolves this issues.
Directly in the script you can edit variables, which archive program you wanna use (ie. lbzip2, pigz, pxz, by default it is lbzip2) and what directories you wanna use.

`After uninstalling the game in steam, always remove physically game directory.
Script can't recognize if there's a directory with uninstalled game, so be carefull, and always check if game is running from steam, if it does't, delete directory before making any backups, for your own safety.`



Installing in linux based systems
---------------------------------

1. create `.bin` folder in your home directory

2. copy file: `steamBackups` to newly created `.bin`

3. go into `.bin` folder

4. `chmod +x steamBackups`

5. go into home directory and

6. add in `.profile` config file this lines:
```
    PATH="$HOME/.bin:$PATH"

    export PATH
```

7. edit script with text editor and set path for variables:

    STEAM_DIR  - if is different than default

    BACKUP_DIR - path to directory where backups will be stored

Relogging may be required.
And that's all, should be working by now.
