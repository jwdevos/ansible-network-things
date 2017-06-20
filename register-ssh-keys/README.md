# register-ssh-keys
The playbook in this directory (playbook-register-ssh-keys.yml) will add the SSH keys for the devices that are in the specified inventory to your known_hosts file.
The playbook assumes a group_var called customer_dir to be available. It contains the name (or directory name in our case, hence the variable name) of the particular customer you are working with. By doing so, it makes the playbook suitable for a multitenancy environment.
You can run the playbook like this:
```
ansible-playbook playbook-register-ssh-keys.yml -i <path-to-inventory>
```
**The code provided here is based largely on the example provided by Ivan Pepelnjak, for which I thank him.**  
**Ivan also runs the site ipspace.net. The site is of interest to anyone concerning him- or herself with networking.**  
**See his original version: https://github.com/ipspace/NetOpsWorkshop/tree/master/tools/ssh-keys**
