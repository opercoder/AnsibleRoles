Role Name
==========
Установка и настройка zabbix агента.  
Сейчас работает для:  
- Astra Linux 1.7
- Astra Linux 1.8

Requirements
------------
wget

Role Variables
--------------
zabbix_server - адрес Zabbix сервера.
zabbix_agent_version - версия Zabbix агента.

Dependencies
------------


Example Playbook
---------------
    - hosts: servers
      roles:
         - opercoder.zabbix-agent

License
-------
BSD

Author Information
------------------
Шумов Алексей
