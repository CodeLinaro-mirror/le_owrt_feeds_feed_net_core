# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release proj_prpl_M1-2022_v0.5.3 - 2022-07-07(13:55:16 +0000)

### Fixes

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): LAN Client does not get IPv4 address on first boot
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): default ODL configures "mod-dns-unbound" but "mod-dns-uci" (dnsmasq) is used

### Changes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Turn off import-dbg
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): split top level ODL

### Other

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Opensource branch proj_prpl_M1-2022

## Release proj_prpl_M1-2022_v0.5.2 - 2022-07-05(13:58:30 +0000)

### Fixes

- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): Fix device reboot to gracefully stop the system
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [dhcpv6client] Not starting (Error_Misconfigured)
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): when bridge br-lan is down eth3 is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): after reboot default services are not loaded
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Index of insertion too big (ssh plugin)
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos][Regression] Queue.TrafficClasses values unexpectedly overwritten
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] fix startup
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] errors when DHCPv6client does not start
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Startup after getting lowerlayer name

### Changes

- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Use a netdev subscription to track the status of the ppp interface and update the status

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo] [FirmwareImage] The deviceinfo module must send a TransferComplete! event when the Downloading is finished.
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Opensource component
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Opensource component
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Opensource component

## Release proj_prpl_M1-2022_v0.5.1 - 2022-06-29(08:04:59 +0000)

### Fixes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): ManufacturerOUI must uses upper-case letters
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [dhcpv6s-manager] Firewall not creating rules for dhcpv6 server
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Should not pass NULL pointer to stat function
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Router] subscribe on a more specific path
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Routing] Disable resolving the netdev name

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Add procps-ng as dependency
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): [amxrt] All amx plugins should start with the -D option
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [amxrt] All amx plugins should start with the -D option
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): [amxrt] All amx plugins should start with the -D option
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [amxrt] All amx plugins should start with the -D option
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [neighbourdiscovery]change netmodel query from netdev-up to netdev-bound
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [amxrt] All amx plugins should start with the -D option
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): [amxrt] All amx plugins should start with the -D option

## Release proj_prpl_M1-2022_v0.5.0 - 2022-06-24(13:26:53 +0000)

### New

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Interface status listening
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [prpl][amx][pcm][dhcpv6server] Definition of Upgrade Persistent DHCPv6 Server Configuration

### Fixes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [tr181-dhcpv4client] fials to load datamodel at startup
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv4client] fials to load datamodel at startup
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [tr181-dhcpv4client] fials to load datamodel at startup

### Other

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] IPv6Prefix listening [add]
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [DHCPv6-manager] DNS servers should be forwarded to client. [add]

## Release proj_prpl_M1-2022_v0.4.1 - 2022-06-24(09:15:18 +0000)

## Release proj_prpl_M1-2022_v0.4.0 - 2022-06-22(19:16:31 +0000)

### New

- [tr181-logical](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical): Component added

### Fixes

- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Datamodel does not load at startup

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

