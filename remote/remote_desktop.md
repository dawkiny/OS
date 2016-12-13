
### Install ```openssh-server```
```sh
sudo apt-get install openssh-server
```



### Install ```xrdp```
```sh
sudo apt-get install xrdp
```

### 
```sh
sudo apt-get update

sudo apt-get install mate-core mate-desktop-environment mate-notification-daemon
```


```sh
sudo sed -i.bak '/fi/a #xrdp multiple users configuration \n mate-session \n' /etc/xrdp/startwm.sh
```
or

```sh
sudo sed -i.bak '/fi/a #xrdp multiple users configuration \n unity \n' /etc/xrdp/startwm.sh
```

