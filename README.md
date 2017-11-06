# steamBackups

Visual console scipt using whiptail for backup/recovery games from steam. 
Initial version, backup and recovery working.

On linux steam archive tool uses only one thread, opens up annoing window and backup multiple games into one directory.
And what if you want to update only one of these games ?

This script resolves this issues.
Directly in to the script you can edit variables which archive program you wanna use (ie. lbzip2, pigz, pxz, by default it is lbzip2) and what directories you wanna use. Maybe in the future usability will be extended.

Script don't recognize if there's a directory with uninstalled game, so be carefull, and always check if game is running from steam, if it does't, delete directory before making any backups, for your own safety.
Best solution to this is to physically remove game directory after uninstalling the game in steam.



You can simply install it this way:

1. create ".bin" folder in your home directory

2. copy files: fileSelector and steamBackups to newly created ".bin"

3. go into ".bin" folder

4. chmod +x fileSelector steamBackups

5. go into home directory and

6. add in ".profile" config file this lines:

    PATH="$HOME/.bin:$PATH"

    export PATH

Relogging may be required.
And that's all, should be working by now.
