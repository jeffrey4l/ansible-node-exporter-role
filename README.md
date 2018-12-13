[![Build Status](https://travis-ci.org/jeffrey4l/ansible-node_exporter-role.svg?branch=master)](https://travis-ci.org/jeffrey4l/ansible-node_exporter-role)

Ansible node exporter Role
==========================

A ansible role to install node_exporter server

Requirements
------------

* ansible >= 2.4

Role Variables
--------------

    node_exporter_bin_path: /opt/node_exporter
    node_exporter_etc_path: /etc/node_exporter
    node_exporter_data_path: /var/lib/node_exporter
    node_exporter_version: 0.17.0

Dependencies
------------

nothing

Example Playbook
----------------

    - name: Install node_exporter server
      hosts: all
      vars:
        node_exporter_version: 0.17.0
      roles:
        - role: ansible-node_exporter-role

License
-------

GPLv3
