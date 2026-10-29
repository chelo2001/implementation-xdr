```mermaid
graph TD
    Kali[Kali Linux VM - Atacante] -->|Simulacion de ataques| Win[Windows VM - Endpoint]
    Win -->|Logs y Telemetria TLS| Ubuntu[Ubuntu Server - XDR Manager]
Figura 1: Topología de red del laboratorio. El agente XDR instalado en la máquina Windows monitorea y envía los registros de eventos mediante una conexión cifrada TLS hacia el servidor XDR en la máquina Ubuntu. La máquina Kali Linux actúa como el agente hostil externo encargado de realizar las simulaciones de ataque para activar las alertas de seguridad.
