# actionpack
packer build scripts for various os's

## packer logging
export PACKER_LOG=1

## windows
got lots of info from https://github.com/StefanScherer/packer-windows

## awx
https://github.com/ansible/awx/blob/devel/INSTALL.md#docker-compose

once system is up. simply install awx
cd /tmp/awx/installer
ansible-playbook -i inventory install.yml

verify the containers
docker ps

## create sha 256
shasum -a 256 {path to iso}