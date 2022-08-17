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
# to only run
go run test.go --configPath ./configfilePath --server <serverip>

#to build and it will generate a binary
go build test.go
<newbinaryname> --configPath ./configfilePath --server <serverip>
```

- create a service using redis-hc.service file.
