# actionpack
packer build scripts for various os's

## packer logging
export PACKER_LOG=1

## packer build command line args
https://www.packer.io/docs/commands/build/

## windows
got lots of info from https://github.com/StefanScherer/packer-windows

also some info here https://www.packer.io/guides/automatic-operating-system-installs/autounattend_windows.html


## awx
packer vm build which gets everything ready for ansible awx install

https://github.com/ansible/awx/blob/devel/INSTALL.md#docker-compose

once system is up. simply install awx
cd /tmp/awx/installer
ansible-playbook -i inventory install.yml

verify the containers
docker ps

## create sha 256
shasum -a 256 {path to iso}
