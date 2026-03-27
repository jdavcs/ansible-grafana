# Grafana

Ansible role for installing and configuring Grafana. Intended primarily for use with a Galaxy installation.

## Role Variables

| variable | default | required |
|:---|:---|:---:|
| grafana_upgrade | `false` ||
| grafana_backup_configs | `false` ||
| grafana_conf_dir | `/etc/grafana` ||
| grafana_data_dir | `/var/lib/grafana` ||
| grafana_log_dir | `/var/log/grafana` ||
| grafana_user |||
| grafana_domain_name || yes |
| grafana_root_url | protocol + domain name + port ||
| grafana_admin_user || yes |
| grafana_admin_pass || yes |
| grafana_secret_key || yes |
| grafana_auth_github |||
| grafana_auth_github_client_id |||
| grafana_auth_github_client_secret |||
| grafana_auth_github_team_ids |||
| grafana_auth_github_allowed_organizations |||
| grafana_email_host |||
| grafana_email_from |||
| grafana_plugins |||

## Dependencies

This role requires the [community.grafana](https://galaxy.ansible.com/ui/repo/published/community/grafana/) collection. To install:

```
ansible-galaxy collection install -r requirements.yml
```

## Example Playbook

```
- hosts: servers
  roles:
     - role: jdavcs.grafana
```

## License

[MIT](LICENSE)
