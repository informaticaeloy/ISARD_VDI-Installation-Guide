# ISARD_VDI-Installation-Guide

### 0. Prerrequisitos

Ubuntu 22.04 Desktop, 2 cores, 8192 RAM, 30GB HD, network bridge

### 1. Instalación de Docker y Docker Compose

sudo apt-get update

sudo apt-get upgrade

sudo apt-get remove docker docker-engine docker.io containerd runc

sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common

curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"

sudo apt-get update -y

sudo apt-get install -y docker.io

sudo apt-get install -y docker-compose

sudo apt-get install -y docker-ce docker-ce-cli containerd.io

sudo apt install python3-pip -y

sudo pip3 install docker-compose

![image](https://user-images.githubusercontent.com/20743678/187424403-9b2b60d5-3033-4c5e-9eb9-62447f76adb2.png)

### 2. Clonar repositorio, build y lanzar docker pull


git clone https://gitlab.com/isard/isardvdi

cd isardivdi

cp isardvdi.cfg.example isardvdi.cfg

sudo ./build.sh 

sudo su

docker-compose pull && docker-compose up -d

![image](https://user-images.githubusercontent.com/20743678/187424608-0b01a0e0-1228-42c0-b904-a99b34d3cd9e.png)
