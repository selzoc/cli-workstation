# CLI Workstation
This repo is used to help setup and maintain a unified cli workstation.

## How to use on Ubuntu (18.04)
For fresh installs on Ubuntu run the following command:

```
$ sudo apt install curl
$ curl -fsSL https://raw.githubusercontent.com/cloudfoundry/cli-workstation/master/install-ubuntu.sh | bash -
# Reboot to pick up new device drivers
$ sudo shutdown -r now
```

To keep the workstation up to date:

```
$ cd ~/workspace/cli-workstation
$ git pull -r
$ ./install-ubuntu.sh
```

### Other things to configure:
- Settings > Mouse & Touchpad > Natural Scrolling : On
- Tilix > Preferences > Profiles > Default > Color > Color Scheme : Monokai Dark

### Things missing from our workstation setup:
- ssh-agent not starting
- concourse-bosh-deployment repo missing
- mouse highlighting for tmux
- remmina confirguration?
- run git-init in repos to update git-duet hook
- zoom
- investigate how to get new git duet-commit (per our techro decision to use the
  new functionality)
