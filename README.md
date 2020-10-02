# Ansible Role: ansible-apps_grafana_exporter

## Description

[![Build Status](https://travis-ci.com/lotusnoir/ansible-apps_grafana_exporter.svg?branch=master)](https://travis-ci.com/lotusnoir/ansible-apps_grafana_exporter)[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)[![Ansible Role](https://img.shields.io/badge/ansible%20role-apps__grafana_exporter-blue)](https://galaxy.ansible.com/lotusnoir/ansible-apps_grafana_exporter/)[![GitHub tag](https://img.shields.io/badge/version-latest-blue)](https://github.com/lotusnoir/ansible-apps_grafana_exporter/tags)

Deploy [grafana_exporter](https://github.com/frodenas/grafana_exporter/) to expose grafana metrics to prometheus.

## Role variables

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `grafana_exporter_version` | 0.1.0 | grafana_exporter version |

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

This project is licensed under MIT License. See [LICENSE](/LICENSE) for more details.
