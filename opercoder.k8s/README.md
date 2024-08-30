Role Name
=========
Установка k8s с помощью kubeadm по официальной документации на debian, ubuntu, astra linux, где используется apt.  
Внимание: с некоторых провайдеров недоступен ресурс https://pkgs.k8s.io/. Тогда надо использовать установку без пакетного менеджера с официального сайта.

Requirements
------------
Установка для Ubuntu/Debian.

Role Variables
--------------


Dependencies
------------
wget

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
Алексей Шумов
