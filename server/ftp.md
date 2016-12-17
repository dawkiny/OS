# FTP(Very Secure FTP)


## Install FTP
```sh
sudo apt install vsftpd
```

## FTP Configuration

```sh
sudo vi /etc/vsftpd.conf




annonymous_enable = NO
local_enable = YES
write_enable = YES
chroot_local_user = YES
allow_writeable_chroot = YES
```

## Restart FTP Service
```sh
sudo service vsftpd restart
```



