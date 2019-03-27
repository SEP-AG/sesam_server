# Sesam Server Installation

This Playbook install a SEPsesam server.

SEP sesam is a backup software soluton with a highly-flexible client-server architecture for heterogeneous
environments. SEP sesam supports with its agents a wide range of operating systems, hypervisors,
databases and applications. While using all necessary APIs for performing consistent online backups,
SEP sesam is certified for many databases and applications, for example, SAP, Oracle, SQL, MySQL,
PostgreSQL, etc. 

### Prerequisites

First please register on our homepage www.sepsoftware.com

Please find the prerequisites on https://wiki.sep.de/wiki/index.php/SEP_sesam_Requirements
The Playbook will check the prerequisites, too.

```
Examples:
PostgresSQL/64-bit installation
Java 11 64-bit
Hard disk space 300GB
```

### Installing

```
Run the ansible playbook
```

## Running the tests

Please set the profile with:
```
. /var/opt/sesam/var/ini/sesam2000.profile
```
Then please check if the sesam server is running:
```
sm_main status
```

Example output:
```
2019-03-27 11:49:09: $Id: 30e8e5a (HEAD, tag: v_4_4_3_64, tag: v4_4_3_4_build, origin/v4_4_3_4, v4_4_3_4) 2018-10-22 10:30:29 +0200 rev:48355
2019-03-27 11:49:09: VERSION='server,4.4.3.64,20181024102809'
2019-03-27 11:49:09: sm_main[25613]
2019-03-27 11:49:09: Arguments: sm_main status
2019-03-27 11:49:09: Found SDS configuration file: "/var/opt/sesam/var/ini/stpd_conf/Sesam-Dedup_2.ini"
2019-03-27 11:49:09: Daemons: ['qm', 'db', 'passd', 'sms', 'stpd', 'ctrl', 'sshd', 'sepuler', 'rmi', 'ui', 'sds-2']
2019-03-27 11:49:09: qm         [  8185]: online
2019-03-27 11:49:09: Found job:   2    db                    0      8202 2019-01-25 16:26:10
2019-03-27 11:49:09: Check DB service. Retry: 1
2019-03-27 11:49:09: db         [  8202]: online
2019-03-27 11:49:09: Found job:   3    passd                 0      8968 2019-01-25 16:26:16
2019-03-27 11:49:09: passd      [  8968]: online
2019-03-27 11:49:09: Found job: 2955    sms                   0     25706 2019-02-28 13:00:43
2019-03-27 11:49:09: sms        [ 25706]: online
2019-03-27 11:49:09: Found job:   5    stpd                  0      9035 2019-01-25 16:26:17
2019-03-27 11:49:09: stpd       [  9035]: online
2019-03-27 11:49:09: Found job:   6    ctrl                  0      9054 2019-01-25 16:26:17
2019-03-27 11:49:09: ctrl       [  9054]: online
2019-03-27 11:49:09: Found job:  27    sshd                  0     15725 2019-01-25 16:29:43
2019-03-27 11:49:09: sshd       [ 15725]: online
2019-03-27 11:49:09: Found job:   8    sepuler               0      9075 2019-01-25 16:26:17
2019-03-27 11:49:09: sepuler    [  9075]: online
2019-03-27 11:49:09: Found job: 1635    rmi                   0     10959 2019-02-12 13:45:41
2019-03-27 11:49:09: rmi        [ 10959]: online
2019-03-27 11:49:09: ui                 : unused
2019-03-27 11:49:09: Found job: 2959    sds-2                 0     26305 2019-02-28 13:01:01
2019-03-27 11:49:09: sds-2      [ 26305]: online
```

## Deployment

www.sepsoftware.com

## Versioning

First version

## Authors

www.sepsoftware.com
service@sep.de
sales@sep.de

## License

Please contact sales@sep.de
