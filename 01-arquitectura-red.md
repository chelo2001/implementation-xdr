```mermaid
graph TD
    Kali[Kali Linux VM - Atacante] -->|Simulacion de ataques| Win[Windows VM - Endpoint]
    Win -->|Logs y Telemetria TLS| Ubuntu[Ubuntu Server - XDR Manager]
