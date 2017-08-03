Restic rest-server
=========

Deploy rest-server for restic.
The intended scheme is that rest-server instances are behind an edge proxy.

Usage
-----

Define `restic_repos` variable.
Start all servers via `systemctl start rest-server.target`

Requirements
------------

None

Role Variables
--------------

```yaml
restic_rest_v: '0.9.4'
restic_repos:
  - path: '/user/home/backup'
    listen: ':8000'
```


License
-------

BSD
