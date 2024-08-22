# Sonarqube Ansible role

This role installs Sonarqube via Docker compose.

## Requirements

None

## Role Variables

All variables are listed below (see also `defaults/main.yml`).

| Name | Description | Default |
| ---: | --- | ---: |
| `sonarqube_image` | The sonarqube docker image | sonarqube |
| `sonarqube_db_image` |  The database docker image | postgres |
| `sonarqube_http_port` | The published HTTP port | 9000 |
| `sonarqube_api_port` | The API port | 9001 |
| `sonarqube_vm_max_map_count` | Elastic search VM max map count | 524288 |
| `sonarqube_fs_file_max` | Elastic search max files opened | 131072 |
| `sonarqube_nofile` | Number of files opened | 131072 |
| `sonarqube_nproc` | Number of processes operened | 8192 |
| `sonarqube_config_path` | Location of the docker compose configuration | /var/local/conf/sonarqube |
| `sonarqube_db_user` | The database user name | changeme |
| `sonarqube_db_password` | The database password | changeme |

Other variables declared in `defaults/main.yml` are defined for internal purposes and you should not touch/change them.

## Dependencies

You need a machine with docker and docker-compose installed.

## Example Playbook

```yml
- hosts: servers
  roles:
      - 'laurivan.sonarqube'
```

## License

This project is licensed under the [MIT](https://opensource.org/licenses/MIT) license - see the [LICENSE](LICENSE) file for details.

![MIT License](https://img.shields.io/badge/license-MIT%20License-brightgreen)

## Author Information

This role was created in 2023 by [Laur Ivan](https://www.laurivan.com).

## Built With

![Ansible](https://img.shields.io/badge/ansible-5.2.0-green.svg)
![Molecule](https://img.shields.io/badge/molecule-3.4.0-green.svg)

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
