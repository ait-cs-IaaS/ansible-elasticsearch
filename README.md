# Ansible installation

## Requirements
- ansible
## Defaults

```
# default elk version
elastic_stack_version: 7.9.3
elastic_stack_version_lock: true

elastic_key_url: "https://artifacts.elastic.co/GPG-KEY-elasticsearch"
elastic_repo: "deb https://artifacts.elastic.co/packages/7.x/apt stable main"
elasticsearch_config_tpl: elasticsearch.yml.j2
elasticsearch_config_dest: /etc/elasticsearch/elasticsearch.yml
```

## Notes
 
> The _elastic_key_url_ and _elastic_repo_ can be found in the defaults folder of _elasticsearch_. 



