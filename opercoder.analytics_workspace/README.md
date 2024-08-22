opercoder.analytics_workspace
=========
Установка на  Astra Linux.
Если версия python не подходит для запуска роли, смотрите https://github.com/opercoder/Linux/blob/main/Ansible/Errors.md.

Requirements
--------------
1. Скачайтие архив tar с сайта производителя.  
2. Скопируйте файл с дистрибутивом на целевой сервер. Расположение файла с дистрибутивом и его имя на целевом сервере укажите в переменной aw_tar_path и aw_tar_filename в файле default/main.yml.  
3. После распаковки имя архива пропишется в файл /opt/aw/app/with_ansible_installed.info дляизбежания повторной установки.
4. Стандартные логин/пароль для входа tech_admin / 123456.

Role Variables
--------------
1. aw_tar_path - расположение дистрибутива с Analytics Workspace на целевом сервере.  
2. aw_version - версия дистрибутива.
3. aw_tar_filename - имя файла архива с дистрибутивом.
4. frontend_url - URL для доступа к приложению.
5. distr_dir - папка с приложением.
6. with_versions_file - файл, хранящий установленные версии.

Dependencies
------------
1. opercoder.nginx

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
Создано Алексеем Шумовым.
