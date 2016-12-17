#SSH

## SSH Server
```sh
sudo apt-get update
sudo apt-get install openssh-server
```

## SSH Server Configuration
```sh
sudo vi /etc/ssh/sshd_config

Port 22 
IgnoreRhosts yes        # Ignore Autologin 
PermitRootLogin no      # Prohibit Login as Root
```

## SSH Client
```sh
sudo apt-get update
sudo apt-get install openssh-client
```
