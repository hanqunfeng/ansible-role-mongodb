Role Name -- mongodb-install
=========

CentOS 7&8 MongoDB 7.0 Installation Role

Requirements
------------

Nothing

Role Variables
--------------
```yml
# vars file for mongodb-install
mongo_install_path: /usr/local/soft
mongo_version: 7.0.6
mongo_replica_set_name: rs0
mongo_port: 27017
# 数据、日志、配置文件、keyFile存储路径
mongo_directory: /mongodb
```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yml
---
- hosts: mongo-servers
  become: yes  # 切换到root用户下执行
  roles:
    - mongodb-install
```

License
-------

BSD

Author Information
------------------

[https://blog.hanqunfeng.com](https://blog.hanqunfeng.com)
