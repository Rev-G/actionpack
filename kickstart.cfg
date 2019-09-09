lang en_US
keyboard us
timezone America/New_York --isUtc
rootpw $1$lB83VVqm$xnLSoEtVY2nLv6EfJj3PC. --iscrypted
#platform x86, AMD64, or Intel EM64T
reboot
text
cdrom
bootloader --location=mbr --append="rhgb quiet crashkernel=auto"
zerombr
clearpart --all --initlabel
autopart
auth --passalgo=sha512 --useshadow
selinux --disabled
firewall --enabled --ssh
firstboot --disable
%packages
@base
-hunspell-en
-yum-rhn-plugin
-fprintd-pam
-ledmon
-smartmontools
-rfkill
-rfkill
-rhnsd
-words
-hunspell
-yum-langpacks
%end
