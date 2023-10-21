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
Add SSH key to ssh-agent.
Install ```gh```.
Setup Github credentials. https://docs.github.com/en/enterprise-cloud@latest/github-cli/github-cli/quickstart

## OSX packages

### Install Homebrew

This pulls Xcode and a bunch of other stuff.

```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Homebrew packages

htop
gh

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
portainer
pihole
- enable queries from whole home network by allowing eth0. make sure 53 is not forwarded for inbound external traffic.
vaultwarden
- install chrome extension https://chrome.google.com/webstore/detail/bitwarden-free-password-m/nngceckbapebfimnlniiiahkandclblb/related





# TODO

https://kopia.io/
https://github.com/ttionya/vaultwarden-backup
https://github.com/drakkan/sftpgo/blob/main/docker/README.md
https://github.com/easyselfhost/self-host/blob/main/docker/dns/docker-compose.yml
