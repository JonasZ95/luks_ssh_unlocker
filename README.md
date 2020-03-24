# Luks SSH Unlocker

The key idea is to use HomeAssistant to check whether a server needs to be unlocked and a key file from a usb stick exists by using **usbmount** to automount an inserted usb drive. 

There are two components:

## ssh_unlock_detect

Can detect if the pc is online. Check whether the given **$KEY_FILE** exists and the given **$HOST** listens on a given **$PORT**.

## ssh_unlock

Unlocks **$DISK_COUNT** - times by using **cryptroot-unlock** with the content of **$KEY_FILE** as key. This used **$HOST_ALIAS** so configure your alias in ~/.ssh/config properly.

## HomeAssistant Example

TODO
