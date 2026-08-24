## VM1 — Wazuh Server

- **OS:** Ubuntu 25.04 (64-bit)
- **RAM:** 9214 MB
- **vCPU:** 4
- **Disco virtual:** 40 GB
- **Sistema de archivos actual:** ~38 GB
- **Red:** NAT
- **IP:** `192.168.1.20`
- **Rol:** Wazuh Server
  <br>


### Componentes instalados

- **Wazuh Manager:** Operativo
- **Wazuh Indexer:** Operativo
- **Wazuh Dashboard:** Operativo

### Estado

**Servidor Wazuh operativo y accesible desde la red del laboratorio.** 
<br>

##Verificación de servicios

Los Servicios fueron comprobados con los comandos.

`sudo systemctl status wazuh-manager --no-pager` <br>
`sudo systemctl status wazuh-indexer --no-pager` <br>
`sudo systemctl status wazuh-dashboard --no-pager` <br>
Los tres servicios indican que estan funcioanndo con: `Active: active (running)`

