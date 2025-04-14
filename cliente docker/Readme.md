Instalar los contenedores

- instalar los servicios con el compando 
``` docker compose up -d ```

- despues en el servidor de prometheus configurar para que pueda leer los datos enviados

hoy lo tenemos todavia al servidor de prometheus en metabase (proximo a ser migrado)
dentro de la carpeta prometheus

Ejemplos:

# Example job for node_exporter
  - job_name: 'srv-test-20-host'
    static_configs:
      - targets: ['10.40.30.20:9100']

# Example job for cadvisor
  - job_name: 'srv-test-20-contenedores'
    static_configs:
      - targets: ['10.40.30.20:8080']
