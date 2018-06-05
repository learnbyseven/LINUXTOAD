# LINUXTOAD
add inux system to active directory
$ yum install sssd realmd oddjob oddjob-mkhomedir adcli samba-common samba-common-tools krb5-workstation openldap-clients policycoreutils-python -y
$ systemctl enable sssd
$ reboot
$ realm join -v --user=admin giriaddns.net (create admin user in AD with member of Administrator group)
or
$ realm join -v giriaddns.net (giriaddns.net is my domain name)
$ realm list (to verify)
Open AD console dsa.msc and list computer 
