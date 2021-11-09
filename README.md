# Ansible Role: elasticsearch

This role installs and configures [elasticsearch](https://www.elastic.co/de/what-is/elasticsearch)

## Defaults

```yaml
# default elk version
elastic_stack_version: 7.9.3
elastic_stack_version_lock: true

elastic_key_url: "https://artifacts.elastic.co/GPG-KEY-elasticsearch"
elastic_repo: "deb https://artifacts.elastic.co/packages/7.x/apt stable main"
elasticsearch_config_tpl: elasticsearch.yml.j2
elasticsearch_config_dest: /etc/elasticsearch/elasticsearch.yml
```

## Notes

> The _elastic_key_url_ and _elastic_repo_ can be found in the defaults folder of [elasticsearch_repo](https://github.com/ait-cs-IaaS/ansible-elasticsearch_repo).

## X-PACK

### Default Roles

- kibana_dashboard_only_user
- apm_system
- watcher_admin
- logstash_system
- rollup_user
- kibana_user
- beats_admin
- remote_monitoring_agent
- rollup_admin
- data_frame_transforms_admin
- snapshot_user
- monitoring_user
- enrich_user
- kibana_admin
- logstash_admin
- machine_learning_user
- data_frame_transforms_user
- machine_learning_admin
- watcher_user
- apm_user
- beats_system
- reporting_user
- transform_user
- kibana_system
- transform_admin
- transport_client
- remote_monitoring_collector
- superuser
- ingest_admin
