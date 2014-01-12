# dokku-pm2

Dokku plugin to utilize the power of pm2.

## Installation

Browse to dokku plugins folder and clone `dokku-pm2`,

```bash
$ cd /var/lib/dokku/plugins
$ git clone https://github.com/likeastore/dokku-pm2
```

## Configuration

Plugin folder contains `default.yaml` file defaults `pm2` configuration for application:

```
mode: cluster
instances: max
```

This would run the application in cluster mode utilizing maximum available CPU's.

## Commands

The list of `pm2` commands exposed by `dokku` interace:

```plain
	dokku pm2:list app
	dokku pm2:monit app
	dokku pm2:logs app
	dokku pm2:status app
	dokku pm2:kill app proc
```

## License

MIT 2014 info@likeastore.com