# Ansible Role: ansible-apps_grafana_exporter

## Description

[![Build Status](https://travis-ci.com/lotusnoir/ansible-apps_grafana_exporter.svg?branch=master)](https://travis-ci.com/lotusnoir/ansible-apps_grafana_exporter)[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen)](https://opensource.org/licenses/Apache-2.0)[![Ansible Role](https://img.shields.io/badge/ansible%20role-apps__grafana_exporter-blue)](https://galaxy.ansible.com/lotusnoir/ansible-apps_grafana_exporter/)[![GitHub tag](https://img.shields.io/badge/version-latest-blue)](https://github.com/lotusnoir/ansible-apps_grafana_exporter/tags)

Deploy [grafana_exporter](https://github.com/frodenas/grafana_exporter/) to expose grafana metrics to prometheus.

## Role variables

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `grafana_exporter_version` | 0.1.0 | grafana_exporter version |
| `grafana_exporter_temp_dir` | /tmp | temporary directory to uncompress package |
| `grafana_exporter_install_dir` | /usr/local/bin | directory to install binary |
| `grafana_exporter_force_install` | false | force install variable |
| `grafana_exporter_listen_port` | 9116 | port to expose prometheus metrics |
| `grafana_uri` | localhost:9092 | port to expose prometheus metrics |


## Examples

	---
	- hosts: apps_grafana_exporter
	  become: yes
	  become_method: sudo
	  gather_facts: yes
	  roles:
	    - role: ansible-apps_grafana_exporter
	  environment: 
	    http_proxy: "{{ http_proxy }}"
	    https_proxy: "{{ https_proxy }}"
	    no_proxy: "{{ no_proxy }}

## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.
