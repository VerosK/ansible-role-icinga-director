# ansible role VerosK.icinga2_director

This role create icinga2 director with postgres

It integrates together with `VerosK.icinga2` and 
`VerosK.icingaweb2` roles.

## Variables

```yaml
icinga2_director_db_type: pgsql
```
Use Postgres as DB

```yaml
icinga2_director_pg_host: localhost
icinga2_director_pg_db: icinga2_director
icinga2_director_pg_user: icinga2_director
icinga2_director_pg_password: 'do-no-use-this-password'
```

Provide parameters to postgres

```yaml
icinga_director_directory: "/usr/share/icingaweb2/modules/director"
```

Directory where to put Director files.

```yaml
icinga_director_version: 'v1.7.1'
icinga_director_installation_method: archive
```
Installation method and version. Currently only `archive`  is
supported, which downloads archive from [Release page][director-releases].


## Notes

Tested on CentOS 7 but can be updated to Debian easily.

Sponsored by [Moravian library](http://www.mzk.cz/)

License: CC0 || 2BSD


[director-releases]: https://github.com/Icinga/icingaweb2-module-director/releases/tag/v1.7.1
