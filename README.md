Filebeat role
=========

Роль для установки filebeat на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

  * Поддерживаются только ОС семейств debian и EL.
  * Elasticsearch
  * Kibana

Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| filebeat_version | "7.14.0" | Параметр, который определяет какой версии filebeat будет установлен |
| elasticsearch_host | "localhost" | Параметр, который определяет ip или имя хоста эластика |
| kibana_host | "0.0.0.0" | Параметр, который определяет ip или имя хоста kibana |


Example Playbook
----------------

    - hosts: all
      roles:
         - { role: filebeat_role }
         - 

License
-------

ect

Author Information
------------------

Ruslan Khozyainov netology 
