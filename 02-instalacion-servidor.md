Para la instalación de la herramienta xdr wazuh, primero se debe descargar e importar la clave GPG del repositorio oficial de wazuh que verifica la autenticidad, integridad del software y permite la confianza entre el sistema operativo y el repositorio externo de wazuh. 
```bash
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo gpg --dearmor -o /usr/share/keyrings/wazuh-archive-keyring.gpg
```
