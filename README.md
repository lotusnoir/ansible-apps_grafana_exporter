# ansible-apps_grafana_exporter

## Description

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_grafana_exporter-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_grafana_exporter)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_grafana_exporter.svg)](https://github.com/lotusnoir/ansible-apps_grafana_exporter/releases/latest)
[![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_grafana_exporter?color=orange&style=flat)](https://galaxy.ansible.com/lotusnoir/apps_grafana_exporter)
[![downloads](https://img.shields.io/ansible/role/d/56086)](https://galaxy.ansible.com/lotusnoir/apps_grafana_exporter)
[![Ansible Quality Score](https://img.shields.io/ansible/quality/56086)](https://galaxy.ansible.com/lotusnoir/apps_grafana_exporter)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)

Deploy [grafana_exporter](https://github.com/frodenas/grafana_exporter/) to expose grafana metrics to prometheus.

## Requirements

none

## Role variables

See [variables](/defaults/main.yml) for more details.

## Examples

        ---
        - hosts: apps_grafana_exporter
          become: true
          become_method: sudo
          gather_facts: true
          roles:
            - role: ansible-apps_grafana_exporter


## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.

