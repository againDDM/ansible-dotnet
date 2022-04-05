# ansible
wh_api ansible infrastructure

```sh
python3 -m pip install -r requirements.txt
ansible-galaxy install -r requirements.yml
ansible-playbook --ask-become-pass playbooks/wh_api.yml
```

TODO:
- mySQL
- добавить в  роль common настройку фаервола, создание пользователей по списку, конфиг ssh демона и раскладку публичных ключей
- logrotate
- мониторинг через [telegraf](https://github.com/influxdata/telegraf) хостовой ОС, nginx, mySQL
- модифицировать роль deploy, добавив healthcheck и fallback
