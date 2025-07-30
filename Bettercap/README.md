# Bettercap

![Bettercap Logo](https://2.bp.blogspot.com/-j4Eq5XSJ2gE/XL2W3AsZUjI/AAAAAAAACXU/gbnBbbuP6AYaL3O83yy9O7VwZZ70t_CRQCLcBGAs/s1600/bettercap.png)

Bettercap is a powerful, flexible, and portable **network monitoring**, **man-in-the-middle**, and **real-time packet manipulation** tool. Built to be extensible and scriptable, it is used by security professionals and penetration testers for a wide range of cybersecurity tasks.

---

## 🔍 Features

- Real-time network sniffer
- ARP spoofing and DNS spoofing
- HTTPS and SSL stripping
- TCP/UDP packet injection
- BLE (Bluetooth Low Energy) sniffing and hijacking
- Wi-Fi monitoring and deauthentication
- Modular and scriptable engine

---

## ⚙️ Requirements

- Linux (Debian-based preferred), macOS, or Windows with WSL
- Go >= 1.11
- libpcap and related network libraries

---

## 🛠️ Installation

### 📦 1. Install Go (if not already installed)

```bash
sudo apt update
sudo apt install golang-go
git clone https://github.com/bettercap/bettercap.git
cd bettercap
make build
sudo make install
wget https://github.com/bettercap/bettercap/releases/latest/download/bettercap_linux_amd64
chmod +x bettercap_linux_amd64
sudo mv bettercap_linux_amd64 /usr/local/bin/bettercap

sudo bettercap

###  Bettercap Commands  

 Basic Commands (within Bettercap session)
net.probe on – Discover live hosts

net.recon on – Scan the LAN network

net.sniff on – Start sniffing

help – Show all available modules and commands