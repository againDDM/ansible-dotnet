# ansible
wh_api ansible infrastructure

```sh
python3 -m pip install -r requirements.txt
ansible-galaxy install -r requirements.yml
ansible-playbook playbooks/wh_api.yml
```

TODO:
- proxy - добавить перезапрос на подписывание сертов при изменении списка доменов, добавить кронячку для перезапросов
- mySQL развёртывание бэкапов
- добавить в  роль common настройку фаервола
- logrotate
- мониторинг через [telegraf](https://github.com/influxdata/telegraf) хостовой ОС, nginx, mySQL
- модифицировать роль deploy, добавив healthcheck и fallback
