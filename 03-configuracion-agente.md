## 03 Configuración del agente en máquina windows para telemetría de logs
---
## Objetivo de la sección
Presentar los pasos para la configuración del agente Wazuh en la máquina windows.

---
## Instalación del agente en máquina windows
Para la instalación del agente, se debe ingresar al siguiente link para descargar el instalador en una máquina windows para después ejecutarlo.
<p align="center">
  <a href="https://documentation.wazuh.com/current/installation-guide/wazuh-agent/wazuh-agent-package-windows.html">Deploying Wazuh agents on Windows endpoints - Wazuh agent</a>
</p>
Luego de la instalación, aparecerá una ventana de configuración como la que se muestra en la figura 1, en donde se debe ingresar la ip de la máquina que ejecuta el XDR Wazuh (una máquina ubuntu en este caso) y una clave de autenticación.
<p align="center">
  <img src="agente-wazuh-config.png" alt="Configuración del agente Wazuh en Windows" width="400">
</p>
<p align="center">
  <em>Figura 1: Configuración del agente Wazuh en el endpoint Windows.</em>
</p>
---

## Obtención de la clave de autenticación
Para la obtención de la clave de autenticación, se debe añadir un nuevo agente en el administrador de XDR Wazuh (máquina ubuntu). Para ello, basta ejecutar el siguiente comando;
```bash
sudo /var/ossec/bin/manage_agents
```
