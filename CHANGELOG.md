# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release v2.2.0 - 2022-01-14(21:25:50 +0000)

### New

- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): Support queries on TR181 paths that are not yet present
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): IP client startup does not always work properly

### Fixes

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Renamed bridging guest default odl to align wth main TR181 bridging manager
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): test coverage in unit test
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): Use default flags
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): Ensure backup path exist on boot

### Changes

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Aligning odl templates according to changes in ip-manager v1.10.0

### Other

- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): - [libfwrules] Document code
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): - [libfwrules] Document code
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): Document code

## Release v2.1.0 - 2022-01-11(20:12:39 +0000)

### New

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Add default file matching hwg config
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): Create DHCPv6 Client mapping in NetModel
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): Retrieve and RequestedOptions
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Create DHCPv4 Client mapping in NetModel
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): Create DHCPv6 Client mapping in NetModel
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): Create DHCPv4 Client mapping in NetModel

### Changes

- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): implement ip client and ip mib
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): create mib_ethernet

## Release v2.0.0 - 2022-01-07(17:10:54 +0000)

### Breaking

- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): rename DMZ parameter SourceInterface to Interface

### New

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Component added
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Integrate with NetDev
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Integrate with tr181-dhcpv4client and tr181-ethernet-manager
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): Automatic interface sensing data model
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Add invalid passwords
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181 Usermanagement] Add private home directory parameter to Users.User
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181 Usermanagement] Add build option for SHA512
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): subscribe to ipv6prefixes
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): use libnetmodel to translate the TR181 interface path to the interface name
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): Support SentOption
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): retrieve requested options from dhcpv4 client (udhcpc)
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): pcm manager should use mod_pcm_scv for backuping itself
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): create mib_ethernet
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Component added
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Set IPv6 address in Linux
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Support for IP.Interface.Enable and IP.Interface.IPv4Enable

### Fixes

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181 Usermanagement] Creating user on GL-B1300 wipes /etc/shadow
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): Remove dictionary
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): implement ip client and ip mib
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): Stats must not be persistent
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): mod_pcm_svc should not use printfs
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): [folder] Cleanup unused rules when invoking fw_folder_delete

### Changes

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Add event and action handler unit tests
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): license: change to BSD-2-Clause-Patent license
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Use BSD-2-Clause-Patent license

### Other

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - Use BSD-2-Clause-Patent license
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [CI] Add libnetmodel as build dependency
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): Use BSD-2-Clause-Patent license

## Release v1.18.0 - 2021-12-16(18:06:47 +0000)

### New

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): queuestats: unit tests
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): Implement IP address queries
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): Add multi object support to mod_pcm_svc
- [libnetmodel](https://gitlab.com/prpl-foundation/components/core/libraries/libnetmodel): Add IP address query functions
- [libdhcpoptions](https://gitlab.com/prpl-foundation/components/core/libraries/libdhcpoptions): Added string to binary conversion for use in DHCPv4 client

### Other

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - Adding unit tests for queue stats
- [libnetmodel](https://gitlab.com/prpl-foundation/components/core/libraries/libnetmodel): Add documentation generation

## Release v1.17.1 - 2021-12-13(22:11:42 +0000)

### Fixes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): notify status change before triggering dnsmasq

### Changes

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): node: Adapt nodes default config and make children and parents not protected.
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): nodes: Use mod_dmext
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): Plugins should only start when wan is up

## Release v1.17.0 - 2021-12-11(11:05:44 +0000)

### New

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implement IPv6Address population
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Add validator for IPv6 prefixes

### Fixes

- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): Use interface name instead of device name for chronyd

### Changes

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): tr181-qos: Make controller and supportedControllers parameter visible in dm

## Release v1.16.0 - 2021-12-09(17:15:54 +0000)

### New

- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): mod-ra-uci: initial commit
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): Add SendBootEvent function to the tr181-device component
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): set flag "netdev" on NetModel interfaces
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): Component added
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Implement reference following to local object

### Fixes

- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): fix loading defaults
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): update changes of ReqOption/SentOption to uci
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): [amx][NetModel] Handle events from entry point events before sending app:start
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Fix memory leaks
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): Fix tests subscription handling

### Changes

- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): Use module mod-dmproxy
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): [amx][NetModel] Add guest interface to defaults

### Other

- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): Skip check of ci jobs
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [CI] Add missing dependency for libdhcpoptions
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [ACL] The IP Manager must have default ACL files configured
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Move component from ambiorix to core on gitlab.com

## Release v1.15.0 - 2021-11-30(20:47:37 +0000)

### New

- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Update the ipv4 instances in ip-manager
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): Implement pcm_json mod (soc)
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): Component added

### Fixes

- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): Cleanup of DM + implementation of missing functions
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): variant cleanup

### Other

- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [CI] Disable g++ compilation
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [CI] Update dependencies

## Release v1.14.0 - 2021-11-30(08:07:45 +0000)

### New

- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Component added

### Fixes

- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): Fix loading of datamodel
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Apply correct default configuration for a guest network
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): Apply correct default configuration for a guest network

### Changes

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): only reload network for static addresses

## Release v1.13.0 - 2021-11-25(16:17:56 +0000)

### New

- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): Component added

### Fixes

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181 Usermanagement] Don't fail on nonexistent groups
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): increase dnsmasq timeout and make it configurable

### Changes

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Add first unit tests
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Use TR181 path in parameter Interface of datamodel

### Other

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): [ACL] Add default ACL file for the QoS Manager

## Release v1.12.0 - 2021-11-24(16:26:05 +0000)

### New

- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): Component added

### Changes

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): enable dhcpv6 guest pool by default

### Other

- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [ACL] The Device plugin must have a default ACL configuration
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [ACL] The TR-181 bridging manager must have default acl files configured
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [ACL] The Routing manager must have default ACL files configured
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [ACL] The DeviceInformation plugin needs to have a default ACL configuration

## Release v1.11.0 - 2021-11-23(17:14:37 +0000)

### New

- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Use mod_netmodel to populate NetModel with the Port instances
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): mod_netmodel populate netmodel hierarchy (Device.IP.)
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): Use mod_netmodel to populate NetModel with the Ethernet instances

### Fixes

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Add mod-netmodel as a dependency

### Other

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [ACL] Usermanagement plugin must provide default Role configuration
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [ACL] The TR181 Firewall manager must have a default ACL configuration
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [ACL] The TR181 Firewall manager must have a default ACL configuration
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implementation of unit tests (using cmocka)
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): [ACL] The EthernetManager must have default ACLS files configured

## Release v1.10.0 - 2021-11-19(16:12:00 +0000)

### New

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): Component added

### Fixes

- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): fix filename typo guest default odl
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): , PCF-405 Disable static routes + enable writing functionality
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [NetDev] resolve netdev crash when adding / deleting devices at a high rate (> 50/s)
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): fix pool update action

### Changes

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181-usermanagement] Always map users to Linux

## Release v1.9.0 - 2021-11-16(19:05:49 +0000)

### New

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [IPManager] Provide (protected) API to set an IPv4 Address instance

### Fixes

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Missing mod-sahtrace dependecy in some components

### Changes

- [mod-vlan-uci](https://gitlab.com/prpl-foundation/components/core/modules/mod-vlan-uci): Move vlan modules from ambiorix folder to core on gitlab.com
- [mod-vlan-ioctl](https://gitlab.com/prpl-foundation/components/core/modules/mod-vlan-ioctl): Move vlan modules from ambiorix folder to core on gitlab.com

### Other

- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): Register on start event
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [CI] Disable g++ compilation

## Release v1.8.1 - 2021-11-15(18:01:36 +0000)

### Fixes

- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): ipv6, attempt to add chain to (not existing) table nat
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): The Firewall level must be configurable in Medium Mode
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): Missing mod-sahtrace dependecy in some components

## Release v1.8.0 - 2021-11-12(15:45:46 +0000)

### New

- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [ip-manager] add guest config

### Fixes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): fix type of ChaddrExclude
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): fix IP range check

## Release v1.7.0 - 2021-11-09(10:53:39 +0000)

### New

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): map users to linux users
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [tr181-firewall] add guest config
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): implement Firewall.X_Prpl_PortTrigger

### Fixes

- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181 Usermanagement] map users to linux users
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [tr181-firewall] add guest config
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add missing dependencies
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): extend fix to all parameters
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): fix writting interface alias to UCI

### Changes

- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): implement Firewall.X_Prpl_PortTrigger
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): set default interface for guest pool

### Other

- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [CI] Disable g++ compilation

## Release v1.6.1 - 2021-11-07(15:06:49 +0000)

## Release v1.6.0 - 2021-11-06(21:22:43 +0000)

### New

- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [tr181-bridging] add guest config to bridging manager
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] add guest config
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [tr181-dhcpv4] add guest config
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): - [libfwrules] Support for ordered rules

### Fixes

- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): Time.CurrentLocalTime is always displayed in UTC time zone
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): fix writing pool to UCI
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): fix modifying Active after applying read-only

## Release v1.5.0 - 2021-11-02(16:47:31 +0000)

### New

- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): Generate event when updating Status, SourceAddress of server in datamodel

### Fixes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): fix applying read only on Status

### Changes

- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): firewall: include in tests, limit max instances

## Release v1.4.0 - 2021-10-28(13:47:17 +0000)

### New

- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): allow rules to match source MAC address
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): Send events when (un)linking interfaces
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [TR181 IP manager] Manage a single Static IPv4Address on a fixed lan interface
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): Add mod_vlan_uci as an optional VLANController
- [mod-vlan-uci](https://gitlab.com/prpl-foundation/components/ambiorix/modules/mod-vlan-uci): Component added

### Fixes

- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): coverity reports DEADCODE
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): Add init script

### Other

- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): [BAF] add support for amx docgen
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): [BAF] add support for amx docgen
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Fix unit tests

## Release v1.3.0 - 2021-10-26(16:38:56 +0000)

### New

- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Add a new protected parameter containing the wifi-iface section name

### Fixes

- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Generate event when changing Status, ..., in datamodel

## Release v1.2.0 - 2021-10-25(18:51:17 +0000)

### New

- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [TR181-DHCPv6 Client] use common datamodel with DHCPv6 server
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): support target NFQUEUE
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): support target NFQUEUE

### Fixes

- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): use common datamodel with DHCPv4 server
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [TR181-DHCPv6 Server] use common datamodel with DHCPv6 client
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): firewall: open port when being configured from uci
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4):  use common datamodel with DHCPv4 client
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): update objects with read-only
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): emit events on Status change

### Changes

- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel): [NetModel] Interface path must start with "Device."
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): enable logging

## Release v1.1.0 - 2021-10-21(15:08:46 +0000)

### New

- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): Component added
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): Fill in Device.Ethernet.Link.{i}. part
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): Create support for VLANTerminations
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): use 'valid' value from lease

### Fixes

- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): set start up order to 22
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): Fetch only objects, skip templates provided by latest libamxb
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): set Client and subobjects as read-only
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): fw_folder_fetch_default_rule failure

## Release v1.0.0 - 2021-10-13(15:14:19 +0000)

### Breaking

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): dhcp(v6) default configuration can be removed

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): NAT.InterfaceSetting status is error
- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): set start up order to 30

## Release v0.20.0 - 2021-10-11(20:04:31 +0000)

### New

- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Implement `mod-routing-uci` logic
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Create `mod-routing-lin` and define controller interface
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Implement `mod-routing-lin` logic
- [pcm-manager](https://gitlab.com/soft.at.home/plugins/tr181-pcm): Add initial registration support + register pcm against itself
- [pcm-manager](https://gitlab.com/soft.at.home/plugins/tr181-pcm): Add PersistentConfiguration datamodel
- [dhcpv6s-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv6s): integrate with firewall

### Fixes

- [tr181-dhcpv4client](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4client): tr181 DHCP Client set start up order to 27
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Add missing deps in .gitlab-ci.yml
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Enable parameter not in sync with status
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Remove forwarding instance the netlink says the route is gone
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): reset dynamic information when forwarding is set static
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Enable not in the right state for automatic detected routes
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): ODL save file issue
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Routing manager does not remove initial IPv\*Forwarding instances

### Changes

- [ip-manager](https://gitlab.com/soft.at.home/plugins/tr181-ip): [TR181 IP] Use amx transactions iso amxd_object_emit_changed
- [dhcpv6s-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv6s): accept multiple lease ips

## Release v0.19.0 - 2021-10-06(14:55:29 +0000)

### New

- [mod-vlan-ioctl](https://gitlab.com/soft.at.home/ambiorix/modules/mod-vlan-ioctl): Component added

### Fixes

- [tr181-dhcpv4client](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4client): Building modules in unit test
- [tr181-dhcpv4client](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4client):  Firewall Support
- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): [Time]Time plugin sometimes does not start

### Other

- [tr181-dhcpv4client](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4client): Opensource component

## Release v0.18.0 - 2021-09-30(16:27:39 +0000)

### New

- [tr181-usermanagement](https://gitlab.com/soft.at.home/plugins/tr181-usermanagement): Component added
- [pcm-manager](https://gitlab.com/soft.at.home/plugins/tr181-pcm): Component added

## Release v0.17.0 - 2021-09-27(21:14:37 +0000)

### New

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): implement Firewall.X_Prpl_Pinhole
- [tr181-dhcpv4client](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4client): Component added

## Release v0.16.0 - 2021-09-22(14:05:03 +0000)

### New

- [libfwrules](https://gitlab.com/soft.at.home/libraries/libfwrules): match rules by connection state

## Release v0.15.0 - 2021-09-17(14:26:53 +0000)

### New

- [tr181-dhcpv6client](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv6client): Component added
- [ethernet-manager](https://gitlab.com/soft.at.home/plugins/tr181-ethernet): Component added
- [mod-dmstats](https://gitlab.com/soft.at.home/ambiorix/modules/mod-dmstats): Component added

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): setService's argument "interface" should support 'Device.IP.Interface.{i}.' paths

## Release v0.14.0 - 2021-09-16(14:54:34 +0000)

### New

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): implement Firewall.X_Prpl_DMZ
- [tr181-device](https://gitlab.com/soft.at.home/plugins/tr181-device): [tr181-Device] add extra documentation to odl
- [tr181-device](https://gitlab.com/soft.at.home/plugins/tr181-device): [GMAP-CLIENT] implement proxy, reboot, factoryreset functions

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): LAN device cannot fetch webpage
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): chain 'INPUT_Services' has no references in table 'nat'
- [tr181-device](https://gitlab.com/soft.at.home/plugins/tr181-device): [TR181-Device] add sahtrace param
- [tr181-device](https://gitlab.com/soft.at.home/plugins/tr181-device): [TR181-Device] add sahtrace param

## Release v0.13.2 - 2021-09-14(16:24:13 +0000)

### Fixes

- [mod-dmext](https://gitlab.com/soft.at.home/ambiorix/modules/mod-dmext): [amxc] add ifdef around when_null_x, when_str_empty_x
- [libfwrules](https://gitlab.com/soft.at.home/libraries/libfwrules): cannot fetch new default rule after calling fw_folder_delete_rules
- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): Add version to `.so` file

## Release v0.13.1 - 2021-09-13(15:06:16 +0000)

### Other

- [libnetmodel](https://gitlab.com/soft.at.home/libraries/libnetmodel): [library NetModel] Add open query functions
- [libfwrules](https://gitlab.com/soft.at.home/libraries/libfwrules): Issue: soft.at.home/libraries/libfwrules#7 delete fails because index is too big

## Release v0.13.0 - 2021-09-10(13:47:38 +0000)

### New

- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): Do not exit the plugin if dnsmasq is not found
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): Implement handling of "Interface" parameter to integrate with other plugins

### Fixes

- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): fix segfault on non existing IP.Interface object
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): fix protovalue being NULL

## Release v0.12.0 - 2021-09-07(19:50:53 +0000)

### New

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): implement NAT.InterfaceSetting to support NAT on the WAN interface
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): default policy of built in chains INPUT and FORWARD must be DROP
- [tr181-bridging](https://gitlab.com/soft.at.home/plugins/tr181-bridging): Create initial ioctl implementation

### Fixes

- [tr181-bridging](https://gitlab.com/soft.at.home/plugins/tr181-bridging): UCI doesn't accept dashes in the names
- [netdev-plugin](https://gitlab.com/soft.at.home/plugins/netdev): PCF-288: [Netdev] crashes when doing a /etc/init.d/network restart

### Other

- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): implement policy masquerade

## Release v0.11.2 - 2021-09-03(15:54:35 +0000)

### Fixes

- [tr181-bridging](https://gitlab.com/soft.at.home/plugins/tr181-bridging): Disable bridges instead of removing them from the uci config

## Release v0.11.1 - 2021-09-01(13:54:18 +0000)

### Fixes

- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): Add debian packages
- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): change name

### Other

- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): [CI] Disable gitlab pages job
- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): [CI] Disable test job
- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): [CI] Enable package generation job
- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): Component '.so' should be versioned

## Release v0.11.0 - 2021-08-30(14:51:06 +0000)

### New

- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions): Component added

### Fixes

- [tr181-bridging](https://gitlab.com/soft.at.home/plugins/tr181-bridging): port status will be Error is the NetDev interface does not yet exist

### Changes

- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Redefine startup order
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): add defaults directory

## Release v0.10.1 - 2021-08-25(16:34:46 +0000)

### Fixes

- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): Update DM accordingly to initially populated objects
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): Avoid spurious lease events, keep only the most recent
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): fix status displayed in Pool, LeaseTime

### Changes

- [netdev-plugin](https://gitlab.com/soft.at.home/plugins/netdev): redefine startup order

### Other

- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): update license

## Release v0.10.0 - 2021-08-25(06:59:50 +0000)

### New

- [wan-manager](https://gitlab.com/soft.at.home/plugins/wan-manager): Component added
- [tr181-bridging](https://gitlab.com/soft.at.home/plugins/tr181-bridging): Configure bridges using UCI and netifd
- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): open/close firewall port for ntp

### Fixes

- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): open/close firewall port for ntp
- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): libfwinterface misidentifies rules as duplicates

### Other

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): missing default policies

## Release v0.9.0 - 2021-08-24(09:58:48 +0000)

### New

- [dhcpv6s-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv6s): odl: add defaults directory

### Fixes

- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): Align time-manager with latest amx libraries

### Other

- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time): Correct changelog

## Release v0.8.2 - 2021-08-20(14:15:34 +0000)

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): policy does not always result in ip(6)tables rules
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): for_each inception is not allowed because of local variable shadowing
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): Index of deletion too big
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Update ubus when route object is removed from DM
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): fix amxd_object_for_each nesting shadowing
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): fix amxd_object_for_each nesting shadowing

## Release v0.8.1 - 2021-08-18(13:48:40 +0000)

### Fixes

- [libfwrules](https://gitlab.com/soft.at.home/libraries/libfwrules): [libfwrules] Pipeline doesn't stop when memory leaks are detected

### Changes

- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Add child object instances directly too root without use of `libamxb`. Cleanup IPv4 and IPv6 routes handling.

### Other

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): Firewall configuration example
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Update changelog style
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing): Create IPv6 Forwarding event based data population

## Release v0.8.0 - 2021-08-16(12:13:19 +0000)

### New

- [dhcpv6s-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv6s): Component added

### Fixes

- [libnetmodel](https://gitlab.com/soft.at.home/libraries/libnetmodel): Fix traces

## Release v0.7.0 - 2021-08-12(16:52:14 +0000)

### New

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): [TR181 Firewall] TR181 chains and rules
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): add debian package generation
- [libnetmodel](https://gitlab.com/soft.at.home/libraries/libnetmodel): Component added

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): iptables rule matches icmptype 1 by default
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): service parameter "Interface" is not used to match packets
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): update copyright headers to be conform with the SPDX specification
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): staticip: fix staticip_remove

### Other

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): Use standard c11
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): Use standard c11
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): [unit testing] better regression testing
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): [unit testing] better regression testing

## Release v0.6.0 - 2021-08-06(14:27:18 +0000)

### New

- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): Server internal eventing

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): Service status is enabled yet no rule found with iptables -L

### Changes

- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): [Startup Order] modify initialization priority

### Other

- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4): Correct CHANGELOG.md formatting

## Release v0.5.1 - 2021-08-05(14:54:46 +0000)

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): [Gitlab CI][Unit tests][valgrind] Pipelines don't stop when memory leaks are detected
- [netdev-plugin](https://gitlab.com/soft.at.home/plugins/netdev): [Netdev] Individual NetDev.Link.{i}. parameters can not be retrieved with ubus-cli
- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): [libfwinterface] Check rule before adding it to the firewall
- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): [libfwinterface] Pipeline doesn't stop when memory leaks are detected

### Other

- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): - [libfwinterface][iptc] Check if a firewall rule exists before an insert or append
- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): Issue: soft.at.home/libraries/libfwinterface#12 baf: add libiptc as a compile and runtime dependency
- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): - [Gitlab CI][Unit tests][valgrind] Pipelines don't stop when memory leaks are detected

## Release v0.5.0 - 2021-08-04(13:00:53 +0000)

### New

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): [TR181 Firewall][Portmapping] port forwarding

### Fixes

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): [tr181-firewall] warn_unused_result during compilation

### Other

- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): add firewall level 'Medium'
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): add firewall level 'Medium'

## Release v0.4.0 - 2021-08-03(20:55:24 +0000)

- [prpl][amx][DHCPv4 Client] Implement a TR181 compliant DHCPv4 Client plugin

## Release v0.3.1 - 2021-08-02(12:51:03 +0000)

## Release v0.3.0 - 2021-07-29(14:57:00 +0000)

### New

- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface): Component added
- [libfwrules](https://gitlab.com/soft.at.home/libraries/libfwrules): Component added
- [mod-dmext](https://gitlab.com/soft.at.home/ambiorix/modules/mod-dmext): Component added
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall): Component added

