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

## Solución de problemas

### Asunto #01 — Corrupción del archivo OpenSearch keystore

Durante el arranque inicial de **Wazuh Indexer**, el servicio falló y no pudo iniciarse correctamente.

El error detectado en los logs fue:

`java.io.EOFException: read past EOF`

El archivo afectado fue:

`/etc/wazuh-indexer/opensearch.keystore`

Al comprobar el archivo, se confirmó que estaba vacío:

- **Tamaño:** 0 bytes
- **Propietario:** `wazuh-indexer`
- **Grupo:** `wazuh-indexer`

La comprobación realizada fue:

```bash
sudo ls -lh /etc/wazuh-indexer/opensearch.keystore
