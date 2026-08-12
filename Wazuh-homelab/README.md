# 🛡️ Wazuh Homelab

Laboratorio práctico de monitorización y detección de eventos de seguridad utilizando Wazuh.<br>

El objetivo de este proyecto es construir un pequeño entorno Blue Team / SOC en el que centralizar eventos de seguridad procedentes de diferentes sistemas operativos, generar actividad controlada y analizar las alertas producidas por Wazuh.

🚧 Project status: In Progress

## 🎯 Objetivo

Los principales objetivos del laboratorio son:<br>

- Desplegar una infraestructura de monitorización de seguridad con Wazuh.
- Configurar un servidor central para la gestión y análisis de eventos.
- Integrar endpoints Linux y Windows mediante Wazuh Agent.
- Centralizar logs y eventos de seguridad.
- Monitorizar eventos de autenticación.
- Detectar actividad potencialmente sospechosa.
- Implementar y probar File Integrity Monitoring (FIM).
- Analizar alertas desde Wazuh Dashboard.
- Investigar eventos de seguridad mediante evidencias recopiladas.
- Relacionar determinados eventos con técnicas de MITRE ATT&CK.
- Documentar el proceso de despliegue, detección e investigación.

## 🏗️ Arquitectura <br>

<img width="549" height="510" alt="image" src="https://github.com/user-attachments/assets/80b7a0d6-3bc9-41e4-b8fa-2e373b1efce1" /><br>

## Componentes
|    Máquina	   |  Sistema operativo	  |              Función                        |
|   -----------  |  ------------------  |  -----------------------------------------  |
|Wazuh Server	   |  Ubuntu Server	      |Gestión, almacenamiento y análisis de eventos|
|Ubuntu Client   |	Ubuntu	            |Endpoint Linux monitorizado                  |
|Windows Client  |	Windows 10	        |Endpoint Windows monitorizado                |

Los tres sistemas estarán conectados mediante una red virtual de laboratorio.
