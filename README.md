# rnrpi-update
rnrpi-update is not rpi-update ! A wrapper to rpi-update which tries to update firmware if applicable and reboot immediately if update succeeds.

rnrpi-update launches rpi-update and let it update the firmware if applicable. If a new firmware is successfully installed, then rnrpi-update shows the output of rpi-update. If no new firmware is available, then rnrpi-update returns silently.
