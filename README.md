# steamBackup

Visual console scipt using whiptail for backup/recovery games from steam. 
Initial version, backup and recovery working.

On linux steam uses only one thread, opens up annoing window and multiple games backups into one directory.

This script resolves this issues.
Directly in the script you can edit variables which archive program you wanna use (ie. lbzip2, pigz, pxz) and
what directories you wanna use. Maybe in the future usability will be extended, to distinguish files to unpack.

Script don't recognize if there are directory without game, so be carefull, and always check if game is running, before making backup. Best solution to this is to physically remove directory after uninstalling in steam.
