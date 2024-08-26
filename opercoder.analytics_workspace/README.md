opercoder.analytics_workspace
=========
По умолчанию запускается в docker на порту 80. В случае необходимости https или какой-либо маршрутищзации можно добавить установку Nginx.  
Установка на  Astra Linux.  
Если версия python не подходит для запуска роли, смотрите https://github.com/opercoder/Linux/blob/main/Ansible/Errors.md.  

Requirements
--------------
1. Скачайтие архив tar с сайта производителя.
2. Скопируйте файл с дистрибутивом на целевой сервер.
3. Заполните переменные в файле default/main.yml:
- aw_tar_path
- aw_version
- frontend_url
- frontend_port
4. После распаковки имя архива пропишется в файл /opt/aw/app/with_ansible_installed.info для избежания повторной установки.
5. Стандартные логин/пароль для входа tech_admin / 123456.

Role Variables
--------------
1. aw_tar_path - расположение дистрибутива с Analytics Workspace на целевом сервере.
2. aw_version - версия дистрибутива.
3. aw_tar_filename - имя файла архива с дистрибутивом.
4. frontend_url - URL для доступа к приложению.
5. frontend_port - порт для доступа к приложению на сервере.
6. distr_dir - папка с приложением.
7. with_versions_file - файл, хранящий установленные версии.

Dependencies
------------

Example Playbook
----------------
- hosts: aw
  roles:
    - opercoder.analytics_workspace
    - opercoder.nginx


License
-------
BSD

Author Information
------------------
Создано Алексеем Шумовым.
