# 01. Arquitectura de Red y Topología

## 🎯 Objetivo de la Sección
Definir la topología del entorno de pruebas virtualizado, identificando los componentes que participan en la simulación de ataques, la recolección de telemetría y la visualización centralizada de alertas de seguridad mediante la solución XDR.

---

## 🏗️ Topología del Laboratorio

```mermaid
graph TD
    Kali[Kali Linux VM - Atacante] -->|Simulacion de ataques| Win[Windows VM - Endpoint]
    Win -->|Logs y Telemetria TLS| Ubuntu[Ubuntu Server - XDR Manager]

