# Hacking_Wifi

<br>

| TABLA DE CONTENIDO     |
| ------------ |
| [Introducción](#Introducción) |
| [Recursos Necesarios](#Recursos-Necesarios) |
| [Configuracion del Entorno](#Configuracion-del-Entorno) |
| [Escaneo de Redes Disponibles](#Escaneo-de-Redes-Disponibles) |
| [Desautenticacion de Dispositivos](#Desautenticacion-de-Dispositivos) |

<br>

### Introduccion

<br>

### Recursos Necesarios

<br>

### Configuracion del Entorno


```cmd
sudo apt update
sudo apt install -y dkms git build-essential

```


```cmd
git clone https://github.com/ulli-kroll/rtl8821au.git
cd rtl8821au
sudo make dkms_install
sudo reboot

```


```cmd
airmon-ng check kill
airmon-ng start wlan0
iwconfig

```


```cmd
airmon-ng stop wlan0
service NetworkManager restart
iwconfig

```

<br>

### Escaneo de Redes Disponibles

<br>

### Desautenticacion de Dispositivos

<br>
