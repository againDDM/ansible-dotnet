# ansible
core_api ansible infrastructure

```sh
python3 -m pip install -r requirements.txt
ansible-galaxy install -r requirements.yml
ansible-playbook --ask-become-pass playbooks/core_api.yml
```

TODO:
- deploy
- mySQL
- logrotate
- мониторинг через [telegraf](https://github.com/influxdata/telegraf) хостовой ОС, nginx, mySQL
- добавить в  роль common настройку фаервола, создание пользователей по списку,конфиг ssh демона и раскладку публичных ключей
- logrotate
