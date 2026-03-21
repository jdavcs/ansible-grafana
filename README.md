-- this readme is a draft --

# Grafana

Ansible role for installing and configuring Grafana.

## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

## Role Variables

- add defaults 

- `grafana_upgrade`: Description. Default: `false`
- `grafana_service_name`: Description. Default: `influxdb`
- `grafana_backup_configs`: Description. Default: `false`
- `grafana_conf_dir`: Description. Default: `/etc/influxdb`
- `grafana_data_dir`: Description. Default: `/var/lib/influxdb`
- `grafana_log_dir`: Description. Default: `/var/lib/influxdb`
- `grafana_user`: Description.
- `grafana_conf_root_url`: required
- `grafana_admin_user`: required
- `grafana_admin_pass`: required
- `grafana_secret_key`: required
- `grafana_domain_name`: required
- `grafana_conf_auth_github`: Description.
- `grafana_conf_auth_github_client_id`: Description.
- `grafana_conf_auth_github_client_secret`: Description.
- `grafana_conf_auth_github_team_ids`: Description.
- `grafana_conf_auth_github_allowed_organizations`: Description.
- `grafana_conf_email_host`: Description.
- `grafana_conf_email_from`: Description.

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: jdavcs.grafana

License
-------

[MIT](LICENSE)
