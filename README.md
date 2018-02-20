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

### Change main VM path

https://askubuntu.com/questions/800824/how-to-change-virtualbox-default-vm-location-in-command-line
- set: `vboxmanage setproperty machinefolder /path/to/directory/`
- check: `vboxmanage list systemproperties | grep folder`
- virtual box: https://superuser.com/questions/408101/virtual-box-not-filling-entire-screen

## Ansible

- [installation](http://docs.ansible.com/ansible/latest/intro_installation.html)
- [unarchive](http://docs.ansible.com/ansible/latest/unarchive_module.html#examples)


## Config reading from bash

- `source "$configfile"` http://wiki.bash-hackers.org/howto/conffile
- [Reading YAML like bash vars](https://medium.com/@mike.reider/handle-bash-config-file-variables-like-a-pro-957dc9a838ed)
 - per one line https://coderwall.com/p/xatm5a/bash-one-liner-to-read-yaml-files
 - other https://stackoverflow.com/questions/5014632/how-can-i-parse-a-yaml-file-from-a-linux-shell-script
 - python shyaml https://github.com/0k/shyaml
 - https://gist.github.com/pkuczynski/8665367
 - collection https://stackoverflow.com/questions/16571739/bash-parsing-variables-from-config-file
 - read per line https://unix.stackexchange.com/questions/175648/use-config-file-for-my-shell-script
 - https://askubuntu.com/questions/743493/best-way-to-read-a-config-file-in-bash
 
## Makefile custom functions

- https://coderwall.com/p/cezf6g/define-your-own-function-in-a-makefile
