# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release proj_prpl_M1-2022_v0.3.1 - 2022-06-22(05:49:31 +0000)

## Release proj_prpl_M1-2022_v0.3.0 - 2022-06-21(13:20:56 +0000)

### New

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Use wld defaults odl generator iso config

## Release proj_prpl_M1-2022_v0.2.1 - 2022-06-21(11:44:19 +0000)

## Release proj_prpl_M1-2022_v0.2.0 - 2022-06-21(07:42:34 +0000)

### New

- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [PCM] PCM-Manager support restore on register and auto sync ctrl
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [PCM] [PPP] [upgrade persistency] Mark PPP Parameters as upgrade persistent

### Fixes

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Rework enable parameters and NetDevName change
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Cleanup defaults
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Toggling IPv6 and setting MTUSize does not work on lla image
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Use netdev-bound instead of netdev-up for NetDevName query
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Weird IP Addresses on interfaces after boot
- [mod-dmstats](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmstats): [ambiorix] dmstats return variant contains the object not the parameter in the get request
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Remove overwriting interface status
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): - [tr181-time] remove debug trace
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [TR181 DHCPv4Client] Change Status parameter after DM is filled in
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [TR181 DHCPv6Client] kill previously launched odhcp6c when fnc start-dhcpv6c is called
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): - [tr181-ppp] Use netmodel queries to find the linux interface
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Plugins not starting at boot
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Update lower layer when creating new wanmodes
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] vlan not disabled when switching from vlan to untagged

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo]ProcessStatus subobject must be supported
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Support of firmware upgrade using TR181
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Add a "public-lan" default IPv4Address instance
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): [amxrt] All amx plugins should start with the -D option
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): mod dmproxy wrong path translation when destination is a parameter in Device.
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Dir path in odl file has one dash too much
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [amxrt] All amx plugins should start with the -D option
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [amxrt] All amx plugins should start with the -D option

## Release proj_prpl_M1-2022_v0.1.0 - 2022-06-07(07:49:31 +0000)

### New

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Add cwmp_plugin template and add port for cwmpd_conn_req in firewall
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Add IPv6Mode = dhcp6 functionality

### Fixes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DISH US HGW][DHCPv4] LAN Client does not get IPv4 address (after hard reset)
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Make AddressingType writable again
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Refactor parameter with object references validation
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected

### Other

- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable

## Release proj_prpl_M1-2022_v0.0.1 - 2022-06-03(14:08:26 +0000)

