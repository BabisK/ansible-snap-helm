Role Name
=========

A role that installs helm from the SNAP repository.

Role Variables
--------------

`helm_snap__state`: One of `present` or `anbsent`. Controls whether the helm snap should be installed or removed.
Default is `present`

`helm_snap__channel`: The channel (version) that will be installed. Default is `stable`.

`helm_snap__autocomplete`: Whether to enable BASH completion. If true, it will create the necessary file in `/etc/bash.completion.d`. Default is `true`.

Example Playbook
----------------
```yaml
- hosts: servers
  roles:
    - role: babisk.ansible-snap-bubectl
```

License
-------

Apache 2.0
