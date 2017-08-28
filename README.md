# unison.service
systemd unit file for unison service

## required config
```
auto=true
batch=true
repeat=5
sshargs=-i /root/.ssh/id_ed25519
```

## installation
1. placed in `/etc/systemd/system/` 
1. reread systemd config: `systemctl daemon-reload`
1. start for testing: `systemctl start unison.service`
1. verify startup: `systemctl status unison.service`
1. enable startup at boot: `systemctl enable unison.service`

