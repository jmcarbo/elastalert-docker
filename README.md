# Elastalert Docker Image
Docker image with Elastalert on Ubuntu.

Requires a link to a Docker container running Elasticsearch using the "elasticsearch_host" alias.
Assumes the use of port 9200 when communicating with Elasticsearch.

# Volumes
/opt/logs       - Elastalert and Supervisord logs will be written to this directory.<br/>
/opt/config     - Elastalert (elastalert_config.yaml) and Supervisord (elastalert_supervisord.conf) configuration files.<br/>
/opt/rules      - Contains Elastalert rules.<br/>

# Environment
SET_CONTAINER_TIMEZONE - Set to "true" (without quotes) to set the tiemzone when starting a container. Default is false.<br/>
CONTAINER_TIMEZONE - Timezone to use in container. Default is Europe/Stockholm.<br/>
