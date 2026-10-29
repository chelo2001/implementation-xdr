```mermaid
graph TD
    subgraph Red de Laboratorio / Virtualización
        Kali[Kali Linux VM <br/> 💻 Máquina Atacante <br/> (Genera ataques y pruebas de concepto)] -->|Simulación de ataques / Tráfico malicioso| Win[Windows VM <br/> 🖥️ Endpoint Monitoreado <br/> (Agente XDR instalado)]
        
        Win -->|Telemetría, Eventos y Logs <br/> (Cifrado TLS)| Ubuntu[Ubuntu Server VM <br/> 🐧 Servidor XDR / Manager <br/> (Dashboard de Visualización y Alertas)]
    end

