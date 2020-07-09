# Pre-requisites

- install [ansible](https://www.ansible.com)

# Configuration

## Fill out necessary fields

- `ansible/inventory/minecraft.yaml`
  - `ansible_host`
  - `ansible_user`
- `ansible/files/whitelist.json`
  - Can leave empty, unless enforcing whitelist
- `ansible/inventory/host_vars/minecraft.yaml`
  - any of the following configuration parameters:
    - `level_name`
    - `motd`
    - `difficulty`
    - `max_tick_time`
    - `view_distance`
    - `white_list`
    - `enforce-whitelist`

## Run

`ansible-playbook -i inventory main.yaml`
