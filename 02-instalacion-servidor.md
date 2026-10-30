# 02. Instalación de herramienta XDR Wazuh
## 🎯 Objetivo de la sección
Presentar los pasos a realizar para la instalación del XDR Wazuh.

---
## 💻 Requisitos del sistema

Para la instalación del servidor Wazuh se utilizó una máquina virtual con las siguientes características:

| Componente | Especificación |
|---|---|
| Sistema operativo | Ubuntu Server 22.04 LTS |
| Memoria RAM | 4 GB |
| Núcleos de CPU | 2 |
| Red | Modo puente (IP 192.168.100.146) |

---
## ⚙️ Pasos para instalación

Para la instalación de la herramienta xdr wazuh, primero se debe descargar e importar la clave GPG del repositorio oficial de wazuh que verifica la autenticidad, integridad del software y permite la confianza entre el sistema operativo y el repositorio externo de wazuh. 
```bash
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo gpg --dearmor -o /usr/share/keyrings/wazuh-archive-keyring.gpg
```
Luego se puede descargar e instalar de manera automatizada la solución xdr wazuh mediante el siguiente comando.
```bash
curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh && sudo bash ./wazuh-install.sh -a -i
```
Después de completarse la instalación, se proporcionarán las credenciales para ingresar al dashboard.

![Credenciales de acceso al dashboard de Wazuh](credenciales-tapadas.png)
