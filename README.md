# jpnewman.elk-topbeat

This is a Ansible role to installs [topbeat](https://www.elastic.co/products/beats/topbeat)

This role is based on role ```topbeat``` [https://github.com/rueian/ansible-elk-example.git]() by Rueian

## Requirements

Ansible 2.x

## Role Variables

|Variable|Description|Default|
|---|---|---|
|```topbeat_version```||1.2.1|
|```topbeat_version_check```||1.2.1|
|```topbeat_platform```||amd64|
|```topbeat_elasticsearch_host```||'localhost:9200'|
|```topbeat_redis_host```||'localhost'|
|```apt_cache_valid_time```||600|

## Dependencies

none

## Example Playbook

    - hosts: servers
      roles:
         - { role: jpnewman.elk-topbeat, tags: ["topbeat"] }

## License

MIT / BSD

## Author Information

John Paul Newman
