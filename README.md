# ubuntu-sshd
Dockerized SSH service, built on top of official Ubuntu images.


## Installed packages
openssh-server

## Config:
PermitRootLogin yes

UsePAM no

exposed port 22

default command: /usr/sbin/sshd -D

root password: p@ssw0rd99

## Run example
```
$ sudo docker run -d -P --name my_sshd yumin9822/ubuntu-sshd:latest
$ sudo docker port my_sshd
22/tcp -> 0.0.0.0:32770
```
