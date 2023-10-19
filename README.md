# General

## Hardware
MacMini

## Configuration

Enable autologin. Requires to disable FileVault.
Enable file and screen sharing.
Change shell to `bash.
```shell
chsh -s /bin/bash
```
Enable SSH login.
Disable bluetooth.

## Installed Applications

docker
- complained with:
```shell
error getting credentials - err: exit status 1, out: `error getting credentials - err: exit status 1, out: `keychain cannot be accessed because the current session does not allow user interaction. The keychain may be locked; unlock it by running "security -v unlock-keychain ~/Library/Keychains/login.keychain-db" and try again
```
- so I had to run:
```shell
security -v unlock-keychain ~/Library/Keychains/login.keychain-db
```

## Installed Docker applications
heimdall
glances
