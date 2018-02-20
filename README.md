# Admin notes

Brief how-to of admin

## Files & dirs

### Search for files

find . -cmin -10 (created less than 10 mins)

### Show dirs size

du -sh *

## Partitions


### Determine partition type

 file -sL /dev/sdc1


### Using partclone for disk imaging

https://partclone.org/usage/partclone.restore.php

http://www.makeuseof.com/tag/2-methods-to-clone-your-linux-hard-drive/
partclone.ext3 -c -d -s /dev/hda1 -o hda1.img


## Vmware 

### Convert Vmware -> Virtualbox

https://www.maketecheasier.com/convert-virtual-machines-vmware-virtualbox/

`ovftool "c:\path\to\original_vm.vmx" "c:\path\to\export.ovf"`

"c:\Program Files (x86)\VMware\VMware Player\OVFTool\ovftool.exe"

## VirtualBox

### [Migration options](https://superuser.com/questions/633431/whats-the-recommended-way-to-move-a-virtualbox-vm-to-another-computer)
