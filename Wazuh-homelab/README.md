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

## 🖥️ Infraestructura
Wazuh Server
Recurso	Configuración
OS	Ubuntu Server 24.04 LTS
CPU	3 vCPU
RAM	6 GB
Storage	25 GB
Hostname	wazuh-server
Role	Wazuh Manager / Indexer / Dashboard

💡 El almacenamiento podrá ampliarse posteriormente si el volumen de eventos y logs del laboratorio aumenta.

Ubuntu Client
Recurso	Configuración
OS	Ubuntu
Role	Endpoint Linux
Agent	Wazuh Agent
Windows Client
Recurso	Configuración
OS	Windows 10
Role	Endpoint Windows
Agent	Wazuh Agent

Windows Client
Recurso	Configuración
OS	Windows 10
Role	Endpoint Windows
Agent	Wazuh Agent
🔧 Tecnologías
Wazuh
Ubuntu Server
Ubuntu Linux
Windows 10
Wazuh Agent
Wazuh Manager
Wazuh Indexer
Wazuh Dashboard
MITRE ATT&CK
Virtualización

## 🚀 Deployment

El despliegue del laboratorio se realizará progresivamente.

Phase 1 — Infrastructure

Crear Wazuh Server

Instalar Ubuntu Server

Actualizar el sistema

Configurar hostname

Configurar red estática

Comprobar conectividad

Instalar Wazuh

Verificar Wazuh Dashboard

Phase 2 — Endpoint Integration

Crear Ubuntu Client

Instalar Wazuh Agent en Ubuntu

Registrar Ubuntu Client

Crear Windows 10 Client

Instalar Wazuh Agent en Windows

Registrar Windows Client

Verificar comunicación de los agentes

Phase 3 — Monitoring

Monitorización de autenticaciones

Monitorización de integridad de archivos

Monitorización de actividad privilegiada

Recopilación de eventos de Windows

Monitorización de PowerShell

Análisis de logs

Phase 4 — Detection & Investigation

Generar eventos controlados

Analizar alertas

Investigar eventos desde Wazuh Dashboard

Identificar indicadores relevantes

Relacionar detecciones con MITRE ATT&CK

Documentar casos de uso

## 🔎 Security Use Cases

Una vez desplegada la infraestructura se crearán diferentes escenarios controlados para comprobar las capacidades de detección de Wazuh.

## 🔐 Use Case 01 — Authentication Monitoring

Objetivo: detectar y analizar eventos relacionados con autenticaciones.

Endpoint:

Ubuntu Client

Actividad a investigar:

Successful authentication
Failed authentication
Repeated authentication failures

Estado:

🚧 Planned

## 📁 Use Case 02 — File Integrity Monitoring

Objetivo: detectar modificaciones en archivos monitorizados.

Se generará actividad controlada sobre determinados archivos y se analizarán los eventos producidos por Wazuh.

Estado:

🚧 Planned

## 🪟 Use Case 03 — Windows Security Events

Objetivo: recopilar y analizar eventos de seguridad generados en Windows 10.

Estado:

🚧 Planned

## ⚡ Use Case 04 — PowerShell Activity

Objetivo: estudiar la visibilidad proporcionada por Wazuh sobre actividad de PowerShell.

Estado:

🚧 Planned

## 🧩 MITRE ATT&CK

Los casos de detección relevantes se relacionarán con técnicas de MITRE ATT&CK.

Por ejemplo:

Endpoint Activity
       │
       ▼
Security Event
       │
       ▼
Wazuh Detection
       │
       ▼
Investigation
       │
       ▼
MITRE ATT&CK Mapping

Esta sección se irá completando a medida que se validen los diferentes casos de uso.

## 📊 Detection & Investigation

Cada caso de detección será documentado siguiendo una estructura común:

Campo	Información
Detection ID	DC-XX
Endpoint	Sistema afectado
Event	Evento observado
Severity	Nivel de severidad
Technique	MITRE ATT&CK
Evidence	Capturas / eventos
Investigation	Análisis realizado
Result	Resultado
Status	Validated / Failed

Esto permitirá mantener una metodología consistente para documentar las diferentes detecciones.

📸 Evidence

Las capturas y evidencias obtenidas durante el laboratorio se almacenarán en:

/screenshots/

Se documentarán, entre otros:

Estado de los agentes.
Wazuh Dashboard.
Alertas generadas.
Eventos de autenticación.
Cambios detectados mediante FIM.
Eventos de Windows.
Investigaciones realizadas.

## 🧠 Lessons Learned

Esta sección se completará durante el desarrollo del laboratorio.

Algunos de los aspectos que se analizarán:

Despliegue de una plataforma SIEM.
Gestión de agentes.
Centralización de eventos.
Diferencias entre monitorización Linux y Windows.
Análisis de alertas.
Priorización de eventos.
Investigación de actividad sospechosa.
Aplicación de MITRE ATT&CK.
Limitaciones y mejoras del laboratorio.

## 🔮 Future Improvements

Posibles ampliaciones futuras del laboratorio:

Añadir más endpoints.
Integrar Sysmon en Windows.
Crear reglas de detección personalizadas.
Crear dashboards específicos.
Simular diferentes técnicas de ataque de forma controlada.
Mejorar la correlación de eventos.
Integrar otras herramientas de seguridad.
Construir escenarios más cercanos a un entorno SOC real.
## 📚 Documentation

La documentación detallada del proyecto se irá organizando en:

docs/ <br>
├── architecture.md <br>
├── installation.md <br>
├── endpoint-deployment.md <br>
├── detection-cases.md <br>
└── lessons-learned.md <br>

## ⚠️ Disclaimer

Este laboratorio se ha creado con fines educativos y de formación en ciberseguridad.

Todas las actividades de generación de eventos y simulación de comportamientos se realizarán exclusivamente dentro del entorno de laboratorio controlado.

## 👤 Project Status

Status: 🚧 In Progress

El laboratorio se encuentra actualmente en fase de despliegue de infraestructura.

Current progress<br>
[████░░░░░░░░░░░░░░░░] Infrastructure <br>
[░░░░░░░░░░░░░░░░░░░░] Endpoint Integration <br>
[░░░░░░░░░░░░░░░░░░░░] Monitoring <br>
[░░░░░░░░░░░░░░░░░░░░] Detection <br>
[░░░░░░░░░░░░░░░░░░░░] Investigation <br>
