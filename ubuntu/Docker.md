# Docker

## Install

```sh
sudo apt-get update
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo apt-key fingerprint 0EBFCD88

sudo add-apt-repository \
    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) \
    stable"

sudo apt-get install docker-ce docker-ce-cli containerd.io
```

Set Docker without using sudo

```sh
# You can use "grep docker /etc/group" to check is successed
sudo usermod -aG docker $(whoami)

# Reboot your computer
sudo reboot
```