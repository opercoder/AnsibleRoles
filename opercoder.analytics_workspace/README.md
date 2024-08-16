opercoder.analytics_workspace
=========
Install on Astra Linux.

Requirements
--------------
1. Скачайтие архив tar с сайта производителя.  
2. Скопируйте файл с дистрибутивом на целевой сервер. Расположение  файла с дистрибутивом  на целевом сервере укажите в переменной {{ aw_tar_file }} в файле default/main.yml.  

Role Variables
--------------
aw_tar_file - расположение дистрибутива с Analytics Workspace на целевом сервере.  

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------
BSD

Author Information
------------------
Сделано Алексеем Шумовым.
