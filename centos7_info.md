# Main Config
## Add user to suo
```usermod -aG wheel username```

## hostname
```sudo hostnamectl set-hostname GCentOS7.blizzow.com```

## DHCP at boot
/etc/sysconfig/network-scripts/ifcfg-ensX

update "ONBOOT" to = "yes"

```ONBOOT=yes```

Need to also look into the "nmcli" command for this. 

## Register the Microsoft RedHat repository
```curl https://packages.microsoft.com/config/rhel/7/prod.repo | sudo tee /etc/yum.repos.d/microsoft.repo```

## Install PowerShell
```sudo yum install -y powershell```

## Install extra releases
```sudo yum install epel-release```

## Install Python3
```sudo yum install python3```

## Install PIP3
```sudo install python3-pip```

## Install pip for pythong 2
```sudo install python-pip```

## Install ansible
```sudo yum install ansible```

# Powershell additions
```Install-Module -Name Pester```

```Install-Module -Name VMWare.PowerCLI```

# Environment vars to consider
```export ansible_python_interpreter=/bin/python3```