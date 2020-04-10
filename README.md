# Ansible: Prometheus + Alertmanager + Grafana

Deploy a full monitoring stack (Prometheus + Alertmanager + Grafana) with Ansible.

## Requirements

* [pipenv](https://github.com/pypa/pipenv)

### Use virtualenv

```
cd virtualenvs
pipenv shell
```

## Deploy

```
ansible-playbook -K -b deploy_stack.yml
```

### Default configuration

* Prometheus: http://localhost:9090
* Alertmanager: http://localhost:9093
* Grafana: http://localhost:3000

## Clean

```
ansible-playbook -K -b clean_stack.yml
```
