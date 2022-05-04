# ansible
wh_api ansible infrastructure

```sh
python3 -m pip install -r requirements.txt
ansible-galaxy install -r requirements.yml
ansible-playbook playbooks/wh_api.yml
```

TODO:
- фиксировать хэш задеплоенного комита и скипать сборку, если нет новых комитов
- proxy - добавить перезапрос на подписывание сертов при изменении списка доменов, добавить кронячку для перезапросов
- добавить в  роль common настройку фаервола
- logrotate
- модифицировать роль deploy, добавив healthcheck и fallback
