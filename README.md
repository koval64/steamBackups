# steamBackup

Visual console scipt using whiptail for backup/recovery games from steam. 
Initial version, backup and recovery working.

On linux steam uses only one thread, opens up annoing window and multiple games backups into one directory.

This script resolves this issues.
Directly in the script you can edit variables which archive program you wanna use (ie. lbzip2, pigz, pxz) and
what directories you wanna use. Maybe in the future usability will be extended, to distinguish files to unpack.

Script don't recognize if there's a directory without game, so be carefull, and always check if game is running from steam, if it does't, delete directory before making any backups, for your own safety.
Best solution to this is to physically remove game directory after uninstalling the game in steam.
