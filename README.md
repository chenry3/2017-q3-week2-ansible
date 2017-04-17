2017 Q3 Unix/Linux 110 A/B Ansible demo

Copy these files into your /etc/ansible directory and:

- install roles from requirements.txt file
```sudo ansible-galaxy install -r requirements.yml```

- install sshpass program
```sudo apt-get install sshpass```

- Add your localhost SSH key fingerprint to your known_hosts file
```ssh localhost hostname``` (and yes accept fingerprint)

- apply the ansible role (using passworded ssh, and sudo)
```ansible-playbook mysql_playbook.yml -u <username> -s -k -K```
