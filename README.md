Restic rest-server
=========

Deploy rest-server for restic.
The intended usage pattern is that rest-server instances are behind an edge proxy,
which would handle authorization and SSL itself, if necessary.


All servers can be started via `systemctl start rest-server.target`

Requirements
------------

None

Role Variables
--------------

```yaml
restic_rest_v: '0.9.4'
restic_rest_repos:
  - path: '/user/home/backup'
    listen: ':8000'
  - path: '/user/home/backup_something_else'
    listen: ':8001'
```


License
-------

BSD
