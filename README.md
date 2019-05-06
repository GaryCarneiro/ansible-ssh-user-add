# User Playbook


This playbook creates users and adds their SSH keys

#  SSH Keys

SSH keys for every user is defined by configuration

```
AuthorizedKeysFile /etc/ssh/authorized_keys/%u.pub

```

Copy the keys into that folder from authorized_keys folder in playbook

# Enabling  / Disabling Users

Users are added by user module with parameter
```state: present ```

Disabling them by opposite paramter
```state: absent```



