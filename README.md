## how to use

### setup
1. Create a `ssh-config`.

The following examples
```
Host default
  HostName 127.0.0.1
  User vagrant
  Port 2222
  UserKnownHostsFile /dev/null
  StrictHostKeyChecking no
  PasswordAuthentication no
  IdentityFile /Users/test/.ssh/test
  IdentitiesOnly yes
  LogLevel FATAL
```

2. write hostname to `hosts` for ansible deploy.

### Usage

- deploy
```
ansible-playbook -i hosts main.yaml
```