# ISARD_VDI-Installation-Guide

### 0. Prerrequisitos

Fedora 36 Workstation VM under VMWare, 2 cores, 8192 RAM, 20GB HD, network bridge

### 1. Preparación de Fedora

> Buscar actualizaciones:

```shell
sudo dnf upgrade --refresh
```

![image](https://user-images.githubusercontent.com/20743678/187608306-bb4c52b0-9f51-4548-825c-d065ae15c1ed.png)

![image](https://user-images.githubusercontent.com/20743678/187608379-4468a0dc-c910-4571-844b-4a26dceea289.png)

> Actualiza el plugin de DNF:

```shell
sudo dnf install dnf-plugin-system-upgrade
```

![image](https://user-images.githubusercontent.com/20743678/187608534-439b69ce-4e03-408a-966f-8e17492ce425.png)




### 2. Instalación de Docker y Docker Compose

sudo apt-get update
