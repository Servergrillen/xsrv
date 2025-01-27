# xsrv

```
  ╻ ╻┏━┓┏━┓╻ ╻
░░╺╋╸┗━┓┣┳┛┃┏┛
  ╹ ╹┗━┛╹┗╸┗┛ 
```

[![](https://gitlab.com/nodiscc/xsrv/badges/master/pipeline.svg)](https://gitlab.com/nodiscc/xsrv/-/pipelines)
[![](https://bestpractices.coreinfrastructure.org/projects/3647/badge)](https://bestpractices.coreinfrastructure.org/projects/3647)
[![](https://img.shields.io/badge/latest%20release-1.3.1-blue)](https://gitlab.com/nodiscc/xsrv/-/releases)
[![](https://img.shields.io/badge/docs-readthedocs-%232980B9)](https://xsrv.readthedocs.io)

**Install, manage and run self-hosted network services and applications on your own server(s).**

This project provides:

- [ansible](https://en.wikipedia.org/wiki/Ansible_%28software%29) [roles](#roles) to install/configure various network services, applications and management tools (sharing, communication, collaboration systems, file storage, multimedia, office/organization, development, automation, infrastructure...)
- an optional [command-line tool](usage.md) for common operations, configuration, deployment and maintenance of your servers
- a template to [get started with a single server](installation.md) in a few minutes


## Roles
<!--BEGIN ROLES LIST-->
- [apache](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/apache) - Apache web server + PHP-FPM interpreter
- [backup](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/backup) - Remote/local backup service (rsnapshot)
- [common](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/common) - Base setup for Debian servers
- [docker](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/docker) - Open source application containerization technology
- [gitea](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/gitea) - Self-hosted Git service/software forge
- [gotty](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/gotty) - Share your terminal as a web application
- [graylog](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/graylog) - Log capture, storage, real-time search and analysis tool
- [homepage](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/homepage) - Simple webserver homepage/dashboard
- [jellyfin](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/jellyfin) - Media solution that puts you in control of your media
- [mariadb](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/mariadb) - MariaDB database engine
- [monitoring](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/monitoring) - Real-time monitoring, alerting and logging system
- [mumble](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/mumble) - Low-latency VoIP/voice chat server
- [nextcloud](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/nextcloud) - file hosting/sharing/synchronization service and collaboration platform
- [openldap](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/openldap) - LDAP directory server
- [postgresql](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/postgresql) - PostgreSQL database engine
- [proxmox](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/proxmox) - Proxmox VE hypervisor configuration
- [rocketchat](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/rocketchat) - Instant messaging & communication platform
- [samba](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/samba) - Cross-platform file sharing server
- [shaarli](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/shaarli) - Bookmarking & link sharing web application
- [transmission](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/transmission) - Transmission Bittorrent client/web interface
- [tt_rss](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/tt_rss) - Tiny Tiny RSS web-based news feed reader
- [valheim_server](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/valheim_server) - Valheim multiplayer server
<!--END ROLES LIST-->

## Screenshots

[![](https://i.imgur.com/pG1xnig.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/monitoring)
[![](https://i.imgur.com/LNaAH2L.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/nextcloud)
[![](https://i.imgur.com/5TXg6vm.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/tt_rss)
[![](https://i.imgur.com/Jlmj0iE.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/shaarli)
[![](https://i.imgur.com/8cAGkf2.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/gitea)
[![](https://i.imgur.com/Imb0dqO.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/transmission)
[![](https://i.imgur.com/6Im61B0.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/mumble)
[![](https://i.imgur.com/REzcZVh.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/openldap)
[![](https://i.imgur.com/Mib9YkX.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/rocketchat)
[![](https://i.imgur.com/5KDvL9Z.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/homepage)
[![](https://i.imgur.com/H3PIWrt.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/jellyfin)
[![](https://i.imgur.com/wa3pkyJ.png)](https://gitlab.com/nodiscc/xsrv/-/tree/master/roles/graylog)

## Source code

- [Gitlab](https://gitlab.com/nodiscc/xsrv)
- [Github](https://github.com/nodiscc/xsrv)


## License

- [GNU GPLv3](https://gitlab.com/nodiscc/xsrv/-/blob/master/LICENSE) unless noted otherwise in individual files/directories
- Documentation is under the [Creative Commons Attribution-ShareAlike 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license


## Documentation

- [Installation](installation.md)
- [Server preparation](installation/server-preparation.md)
- [Controller preparation](installation/controller-preparation.md)
- [First project](installation/first-project.md)
- [Usage](usage.md)
- [List of all configuration variables](configuration-variables.md)
- [Maintenance](maintenance.md)
- [Advanced usage](advanced.md)
- [Contributing](contributing.md)
- [Appendices](appendices.md)
- [Changelog](https://gitlab.com/nodiscc/xsrv/-/blob/master/CHANGELOG.md)



