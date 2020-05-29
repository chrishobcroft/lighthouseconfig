# lighthouseconfig

## Hardware

- 2Gb RAM
- 2 x 2198MHz vCPU
- 50Gb Disk

## Firewall

Expose ports 22, 80, 443, 4221, 4222

## Commands
```
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
sudo nano /etc/fstab
```
Add this to `/etc/fstab`
```
/swapfile swap swap defaults 0 0
```
Then continue
```
sudo apt update && \
sudo apt upgrade -y

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env

git clone https://github.com/sigp/lighthouse.git
cd lighthouse/
git checkout faster-genesis






```
