## 04 reglas y detección de ataques
---
## Objetivo de la sección
Configurar el agente y las reglas en el servidor Wazuh para la detección de un escaneo de puertos

---
## Configuración del agente
Para hacer que el agente pueda leer los logs del firewall de windows se debe editar el archivo de configuración ossec_config y agregar lo siguiente;
```xml
<localfile>
  <location>C:\Windows\System32\LogFiles\Firewall\pfirewall.log</location>
  <log_format>syslog</log_format>
</localfile>
```
