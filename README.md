# unbound-update

Creates and updates unbound local-data conf file, to be included from `unbound.conf`.

Set up .env files for every file to create:
```
$ cp env.example home.domain.tld.env
$ vi home.domain.tld.env
```

## Cron

Run every hour:
```
0 * * * * ./unbound-update >>cron.log 2>&1
```
