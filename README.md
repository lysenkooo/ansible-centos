# CentOS Web Server Playbook

Run on the remote machine:

```sh
# yum update -y
# useradd -m -s /bin/bash deploy
# passwd deploy
# echo 'deploy ALL=(ALL:ALL) NOPASSWD: ALL' > /etc/sudoers
```

Then on local machine:

```sh
$ ssh-copy-id deploy@hostname
$ make provision
```

## Vagrant

Just run:

```sh
make vagrant
```
