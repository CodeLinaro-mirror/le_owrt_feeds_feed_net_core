# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release proj_prpl_M2-2022_v1.2.1 - 2022-08-30(12:46:37 +0000)

### Fixes

- [tr181-xpon](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-xpon): Correct import of the mod-xpon-prpl module

## Release proj_prpl_M2-2022_v1.2.0 - 2022-08-29(19:03:21 +0000)

### New

- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Dynamic handling of network events (PPP)

### Fixes

- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): support multiple servers of DHCP/ppp/router-advertisement
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add MSS rules for ppp interface traffic

## Release proj_prpl_M2-2022_v1.1.0 - 2022-08-29(16:35:34 +0000)

### New

- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): Component added
- [tr181-xpon](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-xpon): Component added

### Fixes

- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Buffer ppp script data in case the lowerlayer interface is still unknown

## Release proj_prpl_M2-2022_v1.0.1 - 2022-08-24(06:42:45 +0000)

### Fixes

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Issues with dm functions not using internal structure

## Release proj_prpl_M2-2022_v1.0.0 - 2022-08-23(19:02:38 +0000)

### Removed

- [libqosmod](https://gitlab.com/prpl-foundation/components/core/libraries/libqosmod): Component removed

### New

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Interface status listening
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [prpl][amx][pcm][dhcpv6server] Definition of Upgrade Persistent DHCPv6 Server Configuration
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implement the stats object
- [libqoscommon](https://gitlab.com/prpl-foundation/components/core/libraries/libqoscommon): Component added
- [libqosnode](https://gitlab.com/prpl-foundation/components/core/libraries/libqosnode): Component added
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [PCM] PCM-Manager support restore on register and auto sync ctrl
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): Component added
- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): Component added
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): It must be possible to load additional iptables fragments files
- [tr181-logical](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical): Component added
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Issue:  HOP-1572 [tr181-ppp] Make module which configures ppp without netifd
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [PCM] [PPP] [upgrade persistency] Mark PPP Parameters as upgrade persistent
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Add IPv6Mode = dhcp6 functionality

### Fixes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): ManufacturerOUI must uses upper-case letters
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): sysinit done optional
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo][NEC WX3000HP] TR69 and LCM failing due to empty DeviceInfo.SerialNumber
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [tr181-DeviceInfo][async] The Download (and Activate) function in DeviceInfo must be marked as async
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DISH US HGW][DHCPv4] LAN Client does not get IPv4 address (after hard reset)
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): static ip address not working
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [tr181-dhcpv4client] fials to load datamodel at startup
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): CI code check warning: use after free
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): dhcp rule missing
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): DHCP v4/v6 managers started alongside clients
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Rework odhcpd_poll_leases
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv4client] fials to load datamodel at startup
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [dhcpv6s-manager] Firewall not creating rules for dhcpv6 server
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): LAN Client does not get IPv4 address on first boot
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): DHCP v4/v6 managers started alongside clients
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Rework enable parameters and NetDevName change
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Make AddressingType writable again
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Cleanup defaults
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Toggling IPv6 and setting MTUSize does not work on lla image
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Use netdev-bound instead of netdev-up for NetDevName query
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Weird IP Addresses on interfaces after boot
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Some volatile data stays persistent if the IP-manager doesn't shutdown properly
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Unit tests are failing
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Prefix is not reboot persistent for IPv6Addresses
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Refactor parameter with object references validation
- [mod-dmstats](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmstats): [ambiorix] dmstats return variant contains the object not the parameter in the get request
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): [PRPL DISH][DataModel] DHCPv4.Server.Pool.1.Client.1.IPv4Address.1.IPAddress doesn't get the new IP address
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Valgrind complains about uninitialized values
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Should not pass NULL pointer to stat function
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Remove overwriting interface status
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Router] subscribe on a more specific path
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Routing] Disable resolving the netdev name
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): - [tr181-time] remove debug trace
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Make lowerlayers parameter writable
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): Fix device reboot to gracefully stop the system
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [TR181 DHCPv4Client] Change Status parameter after DM is filled in
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Datamodel does not load at startup
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): dhcpv4 client is stuck in DHCPStatus==Init
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): DHCP v4/v6 managers started alongside clients
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [TR181 DHCPv6Client] kill previously launched odhcp6c when fnc start-dhcpv6c is called
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [tr181-dhcpv4client] fials to load datamodel at startup
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [dhcpv6client] Not starting (Error_Misconfigured)
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): DHCP v4/v6 managers started alongside clients
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): default ODL configures "mod-dns-unbound" but "mod-dns-uci" (dnsmasq) is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): when bridge br-lan is down eth3 is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): after reboot default services are not loaded
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Index of insertion too big (ssh plugin)
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [tr181-neighbordiscovery] allow icmpv6 packet on the firewall
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Add fw rule faster
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): - [tr181-ppp] Use netmodel queries to find the linux interface
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Datamodel in error while the HGW got an IP from the the PPP server
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] fix installation path of direct module
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos][Regression] Queue.TrafficClasses values unexpectedly overwritten
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Plugins not starting at boot
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] fix startup
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] errors when DHCPv6client does not start
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Update lower layer when creating new wanmodes
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] vlan not disabled when switching from vlan to untagged
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Startup after getting lowerlayer name
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): No dhcp v4 address on LAN

### Changes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Turn off import-dbg
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): split top level ODL
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Do not open port 22 on all interfaces by default
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Use a netdev subscription to track the status of the ppp interface and update the status
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] default ppp module should be uci iso direct

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo]ProcessStatus subobject must be supported
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Add procps-ng as dependency
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Need to scrub components.h on open source
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): sysinit done optiona
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Support of firmware upgrade using TR181
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo] [FirmwareImage] The deviceinfo module must send a TransferComplete! event when the Downloading is finished.
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] IPv6Prefix listening [add]
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [DHCPv6-manager] DNS servers should be forwarded to client. [add]
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): [amxrt] All amx plugins should start with the -D option
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Add a "public-lan" default IPv4Address instance
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [amxrt] All amx plugins should start with the -D option
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): [amxrt] All amx plugins should start with the -D option
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): mod dmproxy wrong path translation when destination is a parameter in Device.
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): amx/mod_sahtrace does not select dynamically stderr or syslog
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Dir path in odl file has one dash too much
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [amxrt] All amx plugins should start with the -D option
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [amxrt] All amx plugins should start with the -D option
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] localtime not changing when timezone changes
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [amxrt] All amx plugins should start with the -D option
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [amxrt] All amx plugins should start with the -D option
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [CDRouter][TOP 100 IPv6][DNS] Open firewall DNS ports on IPv6 address for Lan interface [FIX]
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Opensource component
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Default][IPv6] Add icmpv6 echo accept as default firewall rule
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [neighbourdiscovery]change netmodel query from netdev-up to netdev-bound
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Opensource component
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [amxrt] All amx plugins should start with the -D option
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Opensource component
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): [amxrt] All amx plugins should start with the -D option
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [tr181-usermanagement] Fix behavior for empty passwords

## Release proj_prpl_M1-2022_v0.8.0 - 2022-08-19(13:00:52 +0000)

### New

- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): Component added
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): It must be possible to load additional iptables fragments files

### Fixes

- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): [PRPL DISH][DataModel] DHCPv4.Server.Pool.1.Client.1.IPv4Address.1.IPAddress doesn't get the new IP address
- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): fix stability issue with pwhm amx
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Add fw rule faster

### Other

- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): amx/mod_sahtrace does not select dynamically stderr or syslog
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [tr181-usermanagement] Fix behavior for empty passwords

## Release proj_prpl_M1-2022_v0.7.3 - 2022-08-04(13:36:46 +0000)

### Fixes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): sysinit done optional
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo][NEC WX3000HP] TR69 and LCM failing due to empty DeviceInfo.SerialNumber
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): DHCP v4/v6 managers started alongside clients
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Rework odhcpd_poll_leases
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): DHCP v4/v6 managers started alongside clients
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Prefix is not reboot persistent for IPv6Addresses
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): DHCP v4/v6 managers started alongside clients
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): DHCP v4/v6 managers started alongside clients
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] fix installation path of direct module

### Other

- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] localtime not changing when timezone changes
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [CDRouter][TOP 100 IPv6][DNS] Open firewall DNS ports on IPv6 address for Lan interface [FIX]
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Default][IPv6] Add icmpv6 echo accept as default firewall rule

## Release proj_prpl_M1-2022_v0.7.2 - 2022-07-27(15:29:54 +0000)

### Fixes

- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): dhcpv4 client is stuck in DHCPStatus==Init

## Release proj_prpl_M1-2022_v0.7.1 - 2022-07-26(14:59:49 +0000)

### Fixes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): dhcp rule missing
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Datamodel in error while the HGW got an IP from the the PPP server

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): sysinit done optiona

## Release proj_prpl_M1-2022_v0.7.0 - 2022-07-20(15:11:56 +0000)

### New

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implement the stats object

### Fixes

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Some volatile data stays persistent if the IP-manager doesn't shutdown properly
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [tr181-neighbordiscovery] allow icmpv6 packet on the firewall

### Changes

- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] default ppp module should be uci iso direct

## Release proj_prpl_M1-2022_v0.6.0 - 2022-07-18(07:57:34 +0000)

### New

- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Issue:  HOP-1572 [tr181-ppp] Make module which configures ppp without netifd

### Fixes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [tr181-DeviceInfo][async] The Download (and Activate) function in DeviceInfo must be marked as async
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): static ip address not working
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): CI code check warning: use after free
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Unit tests are failing
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Valgrind complains about uninitialized values
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Make lowerlayers parameter writable
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): No dhcp v4 address on LAN

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Need to scrub components.h on open source
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [amxrt] All amx plugins should start with the -D option

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

