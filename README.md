# tyk-selinux
Example Tyk SELinux with a hardened service file, currently for port 80

run `'/tyk.sh` you may need to set `setenforce 0` 

Trouble shooting:

install `policycoreutils-devel`, `setools` and `setroubleshoot`

commands: 
- `sealert -l "*"` view alerts
- `ausearch -m AVC -ts recent | audit2allow -R` suggested additions
- `> /var/log/audit/audit.log` clear the audit log
