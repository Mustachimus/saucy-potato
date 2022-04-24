This is my attempt to get to grips with Github in general and learn a bit of Ansible and Python, too


These Ansible files are connecting to Cisco's always on Devnet CSR, so as long as the username and password are
correct and the name resolves in DNS, it should work.  Internet connection needed, of course.


Please be aware the cisco_config_diff.yml file requires -D option to work when running the playbook.
You may see "var not defined" error if you don't.



ansible-playbook -D cisco_config_diff.yml -i hosts.yml

-D needed to run diff_against
-i needed to specify hosts file
 
