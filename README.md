# metrics

Подключение к БД настраивается в grafana/config.monitoring 

Для работы proxy_pass grafana, нужно изменить строчку в конфиге grafana.ini, который находится в volume "grafana_data" (/var/lib/docker/volumes/metrics_grafana_data/_data/)

root_url = %(protocol)s://%(domain)s:%(http_port)s/grafana/
