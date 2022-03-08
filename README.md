odoo14
======

Installs a odoo14 instance on a Ubuntu server.


Role Variables
--------------

| Variable                      | Description                                  | Default  |
|-------------------------------|----------------------------------------------|----------|
| odoo_workers                  | Odoo worker instances                        | 2        |
| odoo_cron_threads             | Odoo background worker instances             | 2        |
| odoo_cluster                  | Odoo cluster with more than one dataase      | false    |
| odoo_update                   | Update Odoo database and modules             | true     |
| odoo_disable_database_manager | Don't show password manager                  | true     |
| odoo_list_db                  | Don't list databases on login window         | true     |
| odoo_proxy_mode               | Is Odoo used behind a proxy                  | 2        |
| odoo_cron_threads             | Define background processing threads         | 2        |
| db_name                       | Used database name                           |          |
| db_user                       | Database user                                |          |
| db_host                       | Postgresql database host                     |          |
| db_password                   | Database password                            |          |
[ odoo_queue                    | Enable odoo queue                            | false    |
| odoo_queue_root               | Workers used for root queue                  | 1        |
| odoo_src                      | https://github.com/oerp-at/odoo-oerp-14.0.git|          |
| odoo_dist                     | Odoo distribution                            | 14.0-oerp|
| odoo_branch                   | Odoo branch                                  | 14.0-oerp|

Dependencies
------------

* git-readonly a user defined role for setting up custom git repositories and keys
* https://github.com/oerp-at/ansible-wkhtmltopdf-0.12.6-1.git


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         odoo14


License
-------

BSD
