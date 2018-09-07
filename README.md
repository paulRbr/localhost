## Initial setup of my personnal debian environment

This repository contains a `localhost.yml` Ansible playbook to setup a freshly installed Debian OS with all the tools and configuration I use.

### What's included?

- Common debian packages installation: 
  - Basic packages: **sudo, rsync, curl, git, apt-transport-https, bash-completion, python-pip, htop**
  - Software packages: **byobu (text window manager and terminal multiplexer), emacs (text editor), peek (animated screenshots as GIFs), firefox 61 (internet browser), weechat (IRC client & [Slack client](https://github.com/wee-slack/wee-slack)), kubectl (Kubernetes command-line tool)**
  - Misc packages: **sqlite3, ibus, im-config, pulseaudio, pulseaudio-module-bluetooth, pavucontrol, bluez, bluez-firmware**
  - Smartkey/encryption packages: **pass, gnupg2, gnupg-agent, pinentry-curses, scdaemon, pcscd, yubikey-personalization, libusb-1.0-0-dev**
- Custom [emacs configuration](https://github.com/paulRbr/emacs.d)
- Custom [bash profile configuration](https://github.com/paulRbr/profile)

### Usage

_You will need ansible to be installed to launch the following commands_

Check what will happen

```bash
ansible-playbook --check --diff localhost.yml
```

When happy about the output launch the playbook for real

```bash
ansible-playbook --diff localhost.yml
```

### License

No license, do what you want with the playbook.

### Suggestions?

Do you have a open-source software that you cannot live without? Please [let me know!](https://gitlab.com/paulrbr/localhost/issues)
