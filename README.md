# rnrpi-update
rnrpi-update is not rpi-update ! A wrapper to rpi-update which tries to update firmware if applicable and reboot immediately if update succeeds.

rnrpi-update launches rpi-update and let it update the firmware if applicable. If a new firmware is successfully installed, then rnrpi-update shows the output of rpi-update and reboot immediately. If no new firmware is available, then rnrpi-update returns silently.

Place it in /usr/local/sbin for example and depending of the frequency you want to run it, make a symlink in the right cron folder.

```shell
cp rnrpi-update /usr/local/sbin/
```

`chmod +x /usr/local/sbin/rnrpi-update`

Example to run rnrpi-install monthly :

`ln -s /usr/local/sbin/rnrpi-update /etc/cron.monthly/`
