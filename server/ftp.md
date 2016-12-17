#FTP

```sh
sudo apt install vsftpd
```

```sh
sudo vi /etc/vsftpd.conf




annonymous_enable = NO
local_enable = YES
write_enable = YES
chroot_local_user = YES
allow_writeable_chroot = YES
```

```sh
sudo service vsftpd restart
```



