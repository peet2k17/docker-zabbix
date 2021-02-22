FROM zabbix/zabbix-server-pgsql:ubuntu-5.2-latest

USER root

RUN apt-get -y update && \
    DEBIAN_FRONTEND=noninteractive apt-get -y --no-install-recommends install \
    jq \
    ssh \
    nano \
    htop && \
    apt-get -y autoremove && \
    apt-get -y clean && \
    rm -rf /var/lib/apt/lists/*