# Prometheus Fail2ban Exporter
This exporter uses `fail2ban-client` to get the number of current and total failed connections and banned IPs on a host.

If ran without any arguments, it will export the metrics for all currently enabled jails to `/var/lib/prometheus/node-exporter/fail2ban.prom`.
 
### Usage
```
usage: fail2ban-export.py [-h] [-j JAIL] [-f FILE]

Export fail2ban-client metrics for Prometheus Node Exporter.

optional arguments:
  -h, --help            show this help message and exit
  -j JAIL, --jail JAIL  Jail name to be exported (all jails if omitted).
  -f FILE, --file FILE  File to write metrics to.
```

### Credits
* Hannes Lindner, for writing the [original version](https://github.com/HannesLindner/fail2ban-export)
