# Errors


## `GPG` errors on `apt-get update`

Expired Pub Key Error:
```sh
apt-key list | grep expired

#pub   2048R/BEB6D886 2015-03-27 [expired: 2017-06-04]

sudo apt-key adv --recv-keys --keyserver keys.gnupg.net BEB6D886

#Executing: /tmp/tmp.XluW2QvFlJ/gpg.1.sh --recv-keys
#--keyserver
#keys.gnupg.net
#BEB6D886
#gpg: requesting key BEB6D886 from hkp server keys.gnupg.net
#gpg: key BEB6D886: "home:Horst3180 OBS Project <home:Horst3180@build.opensuse.org>" not changed
#gpg: Total number processed: 1
#gpg:              unchanged: 1

sudo apt update
```

Done.
