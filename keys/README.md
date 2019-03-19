

# PureTEC Keys playbook
This playbook will create a user add it to any group you request and install keys on the users system. 
You can define the passwords of the targets as a variable in the host file and add
all of the systems you want to add keys to as well. 

# Adding a user and group to target system
edit the u.yaml file to create the user you would like to create along with the associated group on each host. 

# Adding your public key to the target system
edit the k.yaml to point to the correct public key file on your local machine. 

# Running the playbook
ansible-playbook keys.yaml calls the 2 playbooks first to add the user, 
second to install the keys on your target systems.

