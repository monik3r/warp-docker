FROM lscr.io/linuxserver/wireguard:latest

RUN mkdir -p /config/wg_confs

COPY generate_config.sh /usr/local/bin/generate_config.sh
RUN chmod +x /usr/local/bin/generate_config.sh

COPY generate-wg-config /etc/s6-overlay/s6-rc.d/generate-wg-config
COPY init-wireguard-confs /etc/s6-overlay/s6-rc.d/init-wireguard-confs
