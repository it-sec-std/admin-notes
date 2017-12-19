# Admin notes

Brief how-to of admin



### Determine partition type

 file -sL /dev/sdc1


### Using partclone for disk imaging

https://partclone.org/usage/partclone.restore.php

http://www.makeuseof.com/tag/2-methods-to-clone-your-linux-hard-drive/
partclone.ext3 -c -d -s /dev/hda1 -o hda1.img
