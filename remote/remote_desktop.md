
### Install ```openssh-server```
```sh
sudo apt-get install openssh-server
```



### Install ```xrdp```
```sh
sudo apt-get install xrdp

```

```sh
sudo apt-get update

sudo apt-get install mate-core mate-desktop-environment mate-notification-daemon

```


```sh
sudo sed -i.bak '/fi/a #xrdp multiple users configuration \n mate-session \n' /etc/xrdp/startwm.sh

```


### WITH UNITY

```sh
wget http://www.c-nergy.be/downloads/tigervncserver_1.6.80-4_amd64.zip
sudo dpkg -i tigervncserver_1.6.80-4_amd64.deb
sudo apt-get install -f
sudo apt-get install xrdp -y
echo unity>~/.xsession
sudo sed -i.bak '/fi/a #xrdp multiple users configuration \n unity \n' /etc/xrdp/startwm.sh

```
and CHANGE xrdp file
``sh
# Set keyboard layout in xrdp sessions 
cd /etc/xrdp 
test=$(setxkbmap -query | awk -F":" '/layout/ {print $2}') 
echo "your current keyboard layout is.." $test
setxkbmap -layout $test 
sudo cp /etc/xrdp/km-0409.ini /etc/xrdp/km-0409.ini.bak 
sudo xrdp-genkeymap km-0409.ini

```

