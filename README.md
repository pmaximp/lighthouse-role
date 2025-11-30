Lighthosue-role
=========

Ansible роль для установки статики [lighthouse](https://github.com/VKCOM/lighthouse.git). Поддерживается работа как с nginx так и apache2.
Конфигурации собираются из диманических template. Необходим установленный nginx или apache2 на хостах.

Role Variables
--------------

| Name | Description | Type | Default |
|------|-------------|------|---------|
| <a name="input_listen_port"></a> [listen\_port](#input\_listen\_port) | Порт для подключения к lighthouse | `number` | `80` |
| <a name="input_web_servers"></a> [web\_servers](#input\_web\_servers) | Веб сервер который используется для lighthouse. apache или nginx | `string` | `"nginx"` |


Example Playbook
----------------

Пример playbook:

    - hosts: lighthouse
      become: true
      roles:
         - lighthosue-role

License
-------

BSD

Author Information
------------------

Perman Maxim
maxim@7perman.ru