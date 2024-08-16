opercoder.analytics_workspace
=========
Установка на  Astra Linux.
Если версия python не подходит для запуска роли, смотрите https://github.com/opercoder/Linux/blob/main/Ansible/Errors.md.

Requirements
--------------
1. Скачайтие архив tar с сайта производителя.  
2. Скопируйте файл с дистрибутивом на целевой сервер. Расположение файла с дистрибутивом и его имя на целевом сервере укажите в переменной aw_tar_path и aw_tar_filename в файле default/main.yml.  

Role Variables
--------------
aw_tar_path - расположение дистрибутива с Analytics Workspace на целевом сервере.  
aw_tar_filename - имя файла дистрибутива с Analytics Workspace на целевом сервере.  

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

- hosts: aw
  roles:
    - opercoder.analytics_workspace

License
-------
BSD

Author Information
------------------
Сделано Алексеем Шумовым.
