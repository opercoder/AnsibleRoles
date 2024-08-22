# Ansible Roles
Здесь храняться роли Ansible для упрощения установки и=системного ПО на сервера.  
Для использования достаточно:  
1. Скачать репозиторий.
2. Создать playbook вида:  
``` bash
- hosts: some-server
  roles:
    - opercoder.analytics_workspace
    - opercoder.nginx
```
3. Создать/исправить конфигурации роли в соответствии с ее описанием.
4. Запустить playbook.
