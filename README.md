# How to
- Edit parameters in the file group_vars/all.yml match with your REALNAME and Kerberos server
- Edit file kerberos_hosts match with your kerberos server

# Run
- $ ansible-playbook --private-key /path/to/key.pem -i kerberos_hosts kerberos_sites.yml --tags="updatentpserver,server"

# Check
- $ kinit admin/admin@REALNAME
- $ klist