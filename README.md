PostgreSQL
=========

通过 ansible 部署在容器下运行的 PostgreSQL 服务。

Installation
------------

`ansible-galaxy install gengxiankun.postgresql`

Dependencies
------------

- [Docker](https://github.com/gengxiankun-galaxy/docker)

Role Variables
--------------

| parameter | description |
| --------- | ----------- |
| OPT_PATH | 服务部署目录 |
| POSTGRES_CONTAINER_NAME | PostgreSQL 容器名称 |
| POSTGRES_PORT | PostgreSQL 对外端口 |
| POSTGRES_PASSWORD | PostgreSQL root 密码 |
| POSTGRES_VOLUME | PostgreSQL 容器数据持久化卷标 |
| POSTGRES_VERSION | PostgreSQL Docker 镜像版本 |

Example Playbook
----------------

    - hosts: servers
      roles:
         - gengxiankun.postgresql

License
-------

BSD

Author Information
------------------

This role was created in 2026 by Xiankun Geng, Learn more about the author's role in [galaxy](https://galaxy.ansible.com/gengxiankun).
