# Redis health check

- create sample config
```shell
redis:
  host: 127.0.0.1
  port: 6379

server:
  bind: 0.0.0.0
  port: 8080
```

- host ip can be passed at run time as well.
```shell
go run test.go --configPath ./configfilePath --server <serverip>
```

- create a service using redis-hc.service file.
