# actionpack
packer build scripts for various os's

## packer logging
export PACKER_LOG=1

##?? 


The solution is to use OEMDRV.iso, ISO disk type. Next OEMDRV disk has to be mounted to VM's SATA controller.

This command creates OEMDV.iso file with volume labeled 'OEMDRV' out of folder, which is exactly what we need.

$ mkisofs -V OEMDRV -o OEMDRV.iso path/to/directory

## windows
got lots of info from https://github.com/StefanScherer/packer-windows

