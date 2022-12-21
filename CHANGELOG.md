# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release proj_prpl_M4.1-2022_v1.0.0 - 2022-12-21(15:33:34 +0000)

### Removed

- [libqosmod](https://gitlab.com/prpl-foundation/components/core/libraries/libqosmod): Component removed

### New

- [debug-information](https://gitlab.com/prpl-foundation/components/utilities/debug-information): Component added
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [tr181-DeviceInfo] Support the DeviceInfo.VendorConfigFile. datamodel
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Issue: HOP-1511[DeviceInfo] Support the DeviceInfo.VendorLogFile. datamodel
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Add BASEMACADDRESS to /etc/environment
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4 Server] Use separtion of concern for uci and dnsmasq
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4s] creation of module to configure dnsmasq without uci for the lla config
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Interface status listening
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [prpl][amx][pcm][dhcpv6server] Definition of Upgrade Persistent DHCPv6 Server Configuration
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): Add default mac addresses for bridges
- [hosts-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-hosts): Component added
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip):  Add IPaddresses reported by NetDev to the DM if they do not yet exist
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implement the stats object
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [TR181 IP] Add support for PPP
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Add a new wan6 instance that will be used by the PPP wan-mode
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [TR181-IP] Add ipv4 and/or ipv6 flags to netdev interfaces in netmodel
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [WANMode] Add default WANModes (Ethernet_DHCP and Ethernet_PPP)
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): First version of the Readme.md
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): IP Manager DSLite defaults
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [tr181][ip] turn on ipv6address for IANA by default
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Adding two parameters to ip prefixes with the relative preferred lifetime and the relative valid lifetime
- [libdhcpoptions](https://gitlab.com/prpl-foundation/components/core/libraries/libdhcpoptions): support option AFTR
- [libfiletransfer](https://gitlab.com/prpl-foundation/components/core/libraries/libfiletransfer): Component added
- [libimtp](https://gitlab.com/soft.at.home/usp/libraries/libimtp): Component added
- [libnetlink-utils](https://gitlab.com/prpl-foundation/components/core/libraries/libnetlink-utils): Component added
- [libpacket-interception](https://gitlab.com/prpl-foundation/components/core/libraries/libpacket-interception): Component added
- [libqoscommon](https://gitlab.com/prpl-foundation/components/core/libraries/libqoscommon): Component added
- [libqosnode](https://gitlab.com/prpl-foundation/components/core/libraries/libqosnode): Component added
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Add validator for check_is_empty_or_in
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): Issue: Adds debian package generation
- [mod-fw-amx](https://gitlab.com/prpl-foundation/components/core/modules/mod-fw-amx): add firewall rules to forward traffic for PCP mapped packets
- [mod-httpaccess-lighttpd](https://gitlab.com/prpl-foundation/components/core/modules/mod-httpaccess-lighttpd): Component added
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [prpl][qos] Integrate new TR-181 parameters for Device.QoS v2.16
- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): Component added
- [packet-interception](https://gitlab.com/prpl-foundation/components/core/plugins/packet-interception): Component added
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [PCM] PCM-Manager support restore on register and auto sync ctrl
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): Update the README
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): Component added
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [tr181-bridgemanager] Fill in LowerLayers parameter for wifi interfaces
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [tr181][Bridging] add wifi ssid to the guest interfaces
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): implement interface stack
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [WANMode] Add default WANModes (Ethernet_DHCP and Ethernet_PPP)
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): support option AFTR
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [tr181][dhcpv6client] store option 23 OPTION_DNS_SERVERS
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Dynamic handling of network events (PPP)
- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): Component added
- [tr181-dslite](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite): Component added
- [tr181-dynamicdns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dynamicdns): Component added
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): It must be possible to load additional iptables fragments files
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): add firewall rules to forward traffic for PCP mapped packets
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add ipv4/6 netmodel flag to netdevname query
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [amx][firewall]It must be possible to configure firewall specific InterfaceSettings.
- [tr181-httpaccess](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-httpaccess): Component added
- [tr181-logical](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical): Component added
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): switched to the logical interface for cpe-wan
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Update the README
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Add ipv4/6 netmodel flag to netdevname query
- [tr181-pcp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcp): Component added
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Issue:  HOP-1572 [tr181-ppp] Make module which configures ppp without netifd
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [PCM] [PPP] [upgrade persistency] Mark PPP Parameters as upgrade persistent
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [TR181-ppp] Create plugin to control pppd
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Integrate new TR-181 parameters for Device.QoS v2.16
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Expand unit tests for node creation
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Integrate netmodel to translate interfaces
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): Update the README
- [tr181-upnp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-upnp): Component added
- [tr181-xpon](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-xpon): Component added
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Add a configuration for the Ethernet_PPP WANmode
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Add IPv6Mode = dhcp6 functionality
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Create support for mixed IPModes
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANMode] Add default WANModes (Ethernet_DHCP and Ethernet_PPP)
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WAN-Manager] Not possible to use Ethernet_PPP with vlan

### Fixes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): ManufacturerOUI must uses upper-case letters
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): sysinit done optional
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo][NEC WX3000HP] TR69 and LCM failing due to empty DeviceInfo.SerialNumber
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [Config] coredump generation should be configurable
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [tr181-DeviceInfo][async] The Download (and Activate) function in DeviceInfo must be marked as async
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4Server] use of query in priv data
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DISH US HGW][DHCPv4] LAN Client does not get IPv4 address (after hard reset)
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): static ip address not working
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [tr181-dhcpv4client] fials to load datamodel at startup
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): CI code check warning: use after free
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): dhcp rule missing
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): DHCP v4/v6 managers started alongside clients
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4 manager] Do not use uci file for default configuration
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4 manager] Unit test rework after modification
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4-manager] uci config does not update if not already present in the dhcp config file
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4 Serever] Only check Enable for the open and close of the firewall
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [DHCPv4 server] unable to retrieve dhcp address on lla config
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4): [Config] coredump generation should be configurable
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Rework odhcpd_poll_leases
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv4client] fials to load datamodel at startup
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [dhcpv6s-manager] Firewall not creating rules for dhcpv6 server
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): LAN Client does not get IPv4 address on first boot
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): DHCP v4/v6 managers started alongside clients
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): Switch clients handling from "delete all - add all" to add, update and remove
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): Unable to add firewall rule returned -1
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [TR181-DHCPv6] memory leak detected
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [DHCPv6 server] change is up query with an lla check
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [DHCPv6 server] Only check Enable for the open and close of the firewall
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [Config] coredump generation should be configurable
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): [lla config] No connection to the board from lan side after a reset hard
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): the interface disable/enable changes more than IFF_UP bit
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): [Config] coredump generation should be configurable
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Rework enable parameters and NetDevName change
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Make AddressingType writable again
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Issues with dm functions not using internal structure
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Cleanup defaults
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Toggling IPv6 and setting MTUSize does not work on lla image
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Use netdev-bound instead of netdev-up for NetDevName query
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Weird IP Addresses on interfaces after boot
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Some volatile data stays persistent if the IP-manager doesn't shutdown properly
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Unit tests are failing
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Prefix is not reboot persistent for IPv6Addresses
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Crash when deleting subscription
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): IP-manager crash when deleting subscription
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): IP-manager crash when deleting subscription
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Autodetected IP addresses should be enabled when added
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): The autodetection of the IP addresses can cause multiple duplicates
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip):  [WANMode] Add default WANModes (Ethernet_DHCP and Ethernet_PPP)
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Wrong ipv6 toggle when switching ipv6 interfaces after enabling of the pppmode in Wan-Manager
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Disable ULA on LLA config
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): No LLA after firstboot
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [Config] coredump generation should be configurable
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [prplOs compatibility] Don't change path and use ip utility according to installed packages
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - [ibsen][mtk] Mediatek config for QoS
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - [libfwinterface] Fix unused variable
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Add missing dependencies
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): [Config] coredump generation should be configurable
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Refactor parameter with object references validation
- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Parameter with object reference to the same data model causes timeout
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): [object mapping]Subcription on root proxy object causes stack overflow
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): dm_proxy segfaults when wrong proxy object path is provided
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): [mod_dmproxy] Search expressions do not work with the device prefix
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): forward output arguments to caller
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): [Prpl] [USP] [Get_Msg] Bad Get_resp message when full path of parameter is requested
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): Delete response is not properly proxied
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): Fix wrong usage of function amxd_path_setf
- [mod-dmstats](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmstats): [ambiorix] dmstats return variant contains the object not the parameter in the get request
- [mod-fw-amx](https://gitlab.com/prpl-foundation/components/core/modules/mod-fw-amx): remove amxm destructor to prevent invalid read
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): [PRPL DISH][DataModel] DHCPv4.Server.Pool.1.Client.1.IPv4Address.1.IPAddress doesn't get the new IP address
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): [TR181 PCM] pcm-manager crashes after firstboot
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): gcc 11.2.0 linker cannot find -lsahtrace
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] Error_Misconfigured Status when AssuredRate is unconfigured
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Valgrind complains about uninitialized values
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Should not pass NULL pointer to stat function
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): [SAHTrace] Use new syntax to prevent ubus config overwrite
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): ImpactedModules not restarted when profile Updated
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Profile not applied after reboot
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Restart via amxp_subproc_t not working [PROVISORY]
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): [multisettings] Using triggers is not effective
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Issue: PROVISORY HOP-2121 Reset ImpactedModules save file when profile is changed
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Revert Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Failing transactions during stats read
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Remove overwriting interface status
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): No connection to lan after firstboot
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): PPP instances never come up
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): bad typecast
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Netdev instability when performing firstboots
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): dslite0 netdev doesn't come up
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [Config] coredump generation should be configurable
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [Config] coredump generation should be configurable
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): gcc 11.2.0 linker cannot find -lsahtrace
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Router] subscribe on a more specific path
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Routing] Disable resolving the netdev name
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): Fixes for PPP default route
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Router] enable parameter automatically goes to 0
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Routing] a 134 firewall rule is made by the routing-manager
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): Handle static routes differently in routing manager
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [Config] coredump generation should be configurable
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): - [tr181-time] remove debug trace
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [Config] coredump generation should be configurable
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Make lowerlayers parameter writable
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Bridges need to be disabled before being removed by the IOCTL module
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Remove wireless parameters from wifi interfaces in the defaults
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [Config] coredump generation should be configurable
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): Fix device reboot to gracefully stop the system
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [PRPL] The Device. object is empty
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [Config] coredump generation should be configurable
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [TR181 DHCPv4Client] Change Status parameter after DM is filled in
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Datamodel does not load at startup
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): dhcpv4 client is stuck in DHCPStatus==Init
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): DHCP v4/v6 managers started alongside clients
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client):  [WANMode] Add default WANModes (Ethernet_DHCP and Ethernet_PPP)
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [WANMode] Add default WANModes (Ethernet_DHCP and Ethernet_PPP)
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): [Config] coredump generation should be configurable
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): Fails to get an address at firstboot when default wan mode is tagged
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client): gcc 11.2.0 linker cannot find -lsahtrace
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [netmodel][DHCPv6Client][getDHCPOption] DHCPv6 option 24 is wrongly parsed
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [TR181 DHCPv6Client] kill previously launched odhcp6c when fnc start-dhcpv6c is called
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [tr181-dhcpv4client] fials to load datamodel at startup
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [dhcpv6client] Not starting (Error_Misconfigured)
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): DHCP v4/v6 managers started alongside clients
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): dhcpv servers fails to create cpe-dhcpvXs-* firewall services on firstboot
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [DHCPv6client] DHCPv6 goes to "Error_Misconfigured" after toggling IP wan enabled
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [TR181-DHCPv6Client] add/delete firewall rule only when enable changes
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): [tr181][dhcpv6c] lifetime seems to be incorrect
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client): gcc 11.2.0 linker cannot find -lsahtrace
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): support multiple servers of DHCP/ppp/router-advertisement
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): default ODL configures "mod-dns-unbound" but "mod-dns-uci" (dnsmasq) is used
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): PPP DNS servers are not configured
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [Config] coredump generation should be configurable
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Use correct option tag when fetching IPv6 DNS server addresses
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): when bridge br-lan is down eth3 is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): after reboot default services are not loaded
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Index of insertion too big (ssh plugin)
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Cannot configure a Port Mapping via TR069, LeaseTime is defined as RO while should be W
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add MSS rules for ppp interface traffic
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Switch the wan interface of the tr181-firewall to the Logical.Interface.1.
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [NeighbourDiscovery][Firewall]Too many ports are opened by the neighbourdiscovery plugin
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Firewall][StealthMode] stealth rules open the firewall by default.
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [amx][firewall] Fix ipv6 issues caused by spoofing protection.
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Config] coredump generation should be configurable
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add missing default ipv6 rules
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [tr181-neighbordiscovery] allow icmpv6 packet on the firewall
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Add fw rule faster
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [NeighbourDiscovery][Firewall]Too many ports are opened by the neighbourdiscovery plugin
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): after boot, GUA but no ipv6 default route, until new RA received
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): - [tr181-ppp] Use netmodel queries to find the linux interface
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Datamodel in error while the HGW got an IP from the the PPP server
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] fix installation path of direct module
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Buffer ppp script data in case the lowerlayer interface is still unknown
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [Config] coredump generation should be configurable
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): Enable core dumps by default
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos][Regression] Queue.TrafficClasses values unexpectedly overwritten
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Segmentation Error when trying to access QoS. datamodel
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Do not require on NetModel.Intf
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Queues are in state Error if the wan cable is not connected
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Queues are in state Error if the wan cable is not connected
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [VLAN][QOS][WNC] Changing the WANMode to vlan, QoS queues creating will fail
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [VLAN][QOS][WNC] Changing the WANMode to vlan, QoS queues creating will fail
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): fail") added the netmodel flag 'eth_intf' to the
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): [Config] coredump generation should be configurable
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Plugins not starting at boot
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [TR181 Usermanagement] Add dependency on lua-amx
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [Config] coredump generation should be configurable
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): gcc 11.2.0 linker cannot find -lsahtrace
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] fix startup
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] errors when DHCPv6client does not start
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [Config] coredump generation should be configurable
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Update lower layer when creating new wanmodes
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] vlan not disabled when switching from vlan to untagged
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Startup after getting lowerlayer name
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): No dhcp v4 address on LAN
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [Config] coredump generation should be configurable
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): LLA address does not come back to IP.Interface.2. when switching back from ppp-mode to wan-mode

### Changes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Turn off import-dbg
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): tests hint regression with dhcpv6 client and/or server data model not present/responding
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): tests hint regression with dhcpv6 client and/or server data model not present/responding
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Make a default IPv6 Configuration for the guest bridge
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - Index of insertion too big
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): Make it possible to proxy individual instances or template objects
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] NTP server on wnc not reachable
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] create more unit tests for time-manager
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] BBF Time Manager Datamodel Evolutions: Time.Server.
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] BBF Time Manager Datamodel Evolutions: Time.Client.
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] create unit tests for uci-chrony module
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [prpl][Timeplugin] The timeserver must not start until the Time client has synced the time correctly.
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): Excessive chronyd restarts
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): split top level ODL
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): enable doc-check
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): enable doc-check
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Hosts] AccessControl block hosts directly in iptables
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Hosts] AccessControl block hosts directly in ip6tables
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [NAT][DSLite] In case dslite is enabled for ipv4, NAT should be disabled
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Do not open port 22 on all interfaces by default
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): upnp service is not available over IPv6
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Use a netdev subscription to track the status of the ppp interface and update the status
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] default ppp module should be uci iso direct
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] Need a transaction on LastWANMode parameter to get notified when changed

### Other

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [USP][CDROUTER] The upgrade firmware tests are failing
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo]ProcessStatus subobject must be supported
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo] Support the DeviceInfo.VendorLogFile. datamodel
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Issue: HOP-1511[DeviceInfo] Support the DeviceInfo.VendorLogFile. datamodel
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Add procps-ng as dependency
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Need to scrub components.h on open source
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): sysinit done optiona
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Improve plugin boot order
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): - [libfiletransfer] add reply handler to request new API arguments
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Support of firmware upgrade using TR181
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): [DeviceInfo] [FirmwareImage] The deviceinfo module must send a TransferComplete! event when the Downloading is finished.
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): DeviceInfo add support for certification authentication for https downloads
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): DeviceInfo add support for certification authentication for https downloads
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Implement swupdate on wnc board
- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Implement swupdate on wnc board
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] IPv6Prefix listening [add]
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [DHCPv6-manager] DNS servers should be forwarded to client. [add]
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet): [amxrt] All amx plugins should start with the -D option
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Add a "public-lan" default IPv4Address instance
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [amxrt] All amx plugins should start with the -D option
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): [IPv6] ULA Address on lan must be disabled by default.
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Improve plugin boot order
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): disable import-dbg
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): When the IP.Interface.2. (wan) is disabled, remove ipv6 addresses form interface [Fix]
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Make Type parameter persistent
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): [Packet Interception] Create the new Packet Interception component
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Correct dependencies
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): [amxrt] All amx plugins should start with the -D option
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): - Standardization of MoCa Low-Level API for prpl
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): mod dmproxy wrong path translation when destination is a parameter in Device.
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] Runtime dependency on libqosnode is missing
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): amx/mod_sahtrace does not select dynamically stderr or syslog
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Dir path in odl file has one dash too much
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Add unit-tests
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Add unit-tests part 2
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): expose bridgetable
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [CI] Fix typo in dependencies
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [amxrt] All amx plugins should start with the -D option
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [TR181][Routing] a 134 firewall rule is made by the routing-manager
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing): [DSLite][Routing] When DSLite is enabled, a default route must be created as well
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] localtime not changing when timezone changes
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [amxrt] All amx plugins should start with the -D option
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): Disable import-dbg in plugins.
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [TR181][Bridging] use ioctl instead of uci [config]
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging): [TR181][Bridging] revert using ioctl instead of uci [config]
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [Device][DMProxy] Integration of new dmproxy module in prpl.
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): Improve unit testing of the tr181-device plugin.
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [Device][SSH] SSH is no longer correctly mapped to Device.SSH
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [HTTPAccess] Integration of HTTP Access plugin
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [Device] PCP and the DSLite data model must be mapped to Device.PCP/DSlite.
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): add Security to Device.Security datamodel
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [Packet Interception] Create the new Packet Interception component
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device): [Automatic Testing] Add simple checks for the Device.X data model
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [amxrt] All amx plugins should start with the -D option
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): [CDRouter][TOP 100 IPv6][DNS] Open firewall DNS ports on IPv6 address for Lan interface [FIX]
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): set import-dbg to false
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Opensource component
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [Default][IPv6] Add icmpv6 echo accept as default firewall rule
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [amx][firewall] Implement Spoofing protection on specific InterfaceSettings.
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [tr181-firewall] ip6tables-restore is broken
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): [IPv6][Firewall] IPv6 connectivity is broken by spoofing protection feature
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add different firewall policies for IPv4 and IPv6
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [neighbourdiscovery]change netmodel query from netdev-up to netdev-bound
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Opensource component
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [amxrt] All amx plugins should start with the -D option
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Opensource component
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Update documentation
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement): [amxrt] All amx plugins should start with the -D option
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): [tr181-usermanagement] Fix behavior for empty passwords
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): set import-dbg to false

## Release proj_prpl_M4-2022_v1.5.1 - 2022-12-20(13:15:09 +0000)

## Release proj_prpl_M4-2022_v1.5.0 - 2022-12-20(10:20:22 +0000)

### New

- [hosts-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-hosts): Component added

## Release proj_prpl_M4-2022_v1.4.1 - 2022-12-20(09:36:46 +0000)

### Fixes

- [tr181-dynamicdns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dynamicdns): [DynDNS] Crash when entering wrong interface reference
- [tr181-dynamicdns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dynamicdns): [Config] coredump generation should be configurable
- [tr181-dynamicdns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dynamicdns): [DynDNS] Crash when removing a Client instance

## Release proj_prpl_M4-2022_v1.4.0 - 2022-12-19(15:29:23 +0000)

### New

- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): Add validator for check_is_empty_or_in

## Release proj_prpl_M4-2022_v1.3.3 - 2022-12-16(10:37:22 +0000)

### Fixes

- [debug-information](https://gitlab.com/prpl-foundation/components/utilities/debug-information): Improve getDebugInformation prplOs compatibility
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [Config] coredump generation should be configurable

### Changes

- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): Excessive chronyd restarts

### Other

- [debug-information](https://gitlab.com/prpl-foundation/components/utilities/debug-information): Add missing opensource license
- [debug-information](https://gitlab.com/prpl-foundation/components/utilities/debug-information): add boot measure script

## Release proj_prpl_M4-2022_v1.3.2 - 2022-12-13(19:34:12 +0000)

### Changes

- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] create unit tests for uci-chrony module
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [prpl][Timeplugin] The timeserver must not start until the Time client has synced the time correctly.

## Release proj_prpl_M4-2022_v1.3.1 - 2022-12-13(15:53:00 +0000)

### Fixes

- [tr181-dslite](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite): Correct linking with /opt/prplos

## Release proj_prpl_M4-2022_v1.3.0 - 2022-12-13(10:48:28 +0000)

### New

- [tr181-pcp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcp): Component added

### Fixes

- [libnetlink-utils](https://gitlab.com/prpl-foundation/components/core/libraries/libnetlink-utils): Correct syntax for option to compile with libraries installed at /opt/prplos

## Release proj_prpl_M4-2022_v1.2.2 - 2022-12-12(08:11:07 +0000)

### Fixes

- [tr181-dslite](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite): [Config] coredump generation should be configurable

### Changes

- [tr181-dslite](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite): Fix issue with Enable parameters

### Other

- [tr181-dslite](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite): Add runtime dependencies "kmod-ip6-tunnel" and "kmod-iptunnel6"

## Release proj_prpl_M4-2022_v1.2.1 - 2022-12-11(18:34:19 +0000)

## Release proj_prpl_M4-2022_v1.2.0 - 2022-12-11(17:43:00 +0000)

### New

- [libimtp](https://gitlab.com/soft.at.home/usp/libraries/libimtp): Component added
- [libnetlink-utils](https://gitlab.com/prpl-foundation/components/core/libraries/libnetlink-utils): Component added
- [libpacket-interception](https://gitlab.com/prpl-foundation/components/core/libraries/libpacket-interception): Component added
- [packet-interception](https://gitlab.com/prpl-foundation/components/core/plugins/packet-interception): Component added

### Fixes

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - [ibsen][mtk] Mediatek config for QoS
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - [libfwinterface] Fix unused variable
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Add missing dependencies

### Other

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): [Packet Interception] Create the new Packet Interception component

## Release proj_prpl_M4-2022_v1.1.1 - 2022-12-11(14:08:18 +0000)

## Release proj_prpl_M4-2022_v1.1.0 - 2022-12-01(13:24:57 +0000)

### New

- [debug-information](https://gitlab.com/prpl-foundation/components/utilities/debug-information): Component added

## Release proj_prpl_M4-2022_v1.0.0 - 2022-12-01(08:41:43 +0000)

### Removed

- [libqosmod](https://gitlab.com/prpl-foundation/components/core/libraries/libqosmod): Component removed

### New

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Interface status listening
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [prpl][amx][pcm][dhcpv6server] Definition of Upgrade Persistent DHCPv6 Server Configuration
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implement the stats object
- [libqoscommon](https://gitlab.com/prpl-foundation/components/core/libraries/libqoscommon): Component added
- [libqosnode](https://gitlab.com/prpl-foundation/components/core/libraries/libqosnode): Component added
- [mod-httpaccess-lighttpd](https://gitlab.com/prpl-foundation/components/core/modules/mod-httpaccess-lighttpd): Component added
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [prpl][qos] Integrate new TR-181 parameters for Device.QoS v2.16
- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): Component added
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [PCM] PCM-Manager support restore on register and auto sync ctrl
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): Component added
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Dynamic handling of network events (PPP)
- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): Component added
- [tr181-dslite](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dslite): Component added
- [tr181-dynamicdns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dynamicdns): Component added
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): It must be possible to load additional iptables fragments files
- [tr181-httpaccess](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-httpaccess): Component added
- [tr181-logical](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical): Component added
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Issue:  HOP-1572 [tr181-ppp] Make module which configures ppp without netifd
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [PCM] [PPP] [upgrade persistency] Mark PPP Parameters as upgrade persistent
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Integrate new TR-181 parameters for Device.QoS v2.16
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Expand unit tests for node creation
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Integrate netmodel to translate interfaces
- [tr181-upnp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-upnp): Component added
- [tr181-xpon](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-xpon): Component added
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
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Issues with dm functions not using internal structure
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
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] Error_Misconfigured Status when AssuredRate is unconfigured
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Valgrind complains about uninitialized values
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Should not pass NULL pointer to stat function
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Revert Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Failing transactions during stats read
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Remove overwriting interface status
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): No connection to lan after firstboot
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): PPP instances never come up
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): bad typecast
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Netdev instability when performing firstboots
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
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): support multiple servers of DHCP/ppp/router-advertisement
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): default ODL configures "mod-dns-unbound" but "mod-dns-uci" (dnsmasq) is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): when bridge br-lan is down eth3 is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): after reboot default services are not loaded
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Index of insertion too big (ssh plugin)
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add MSS rules for ppp interface traffic
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [tr181-neighbordiscovery] allow icmpv6 packet on the firewall
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Add fw rule faster
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): - [tr181-ppp] Use netmodel queries to find the linux interface
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Datamodel in error while the HGW got an IP from the the PPP server
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] fix installation path of direct module
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Buffer ppp script data in case the lowerlayer interface is still unknown
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): Enable core dumps by default
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos][Regression] Queue.TrafficClasses values unexpectedly overwritten
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Segmentation Error when trying to access QoS. datamodel
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Do not require on NetModel.Intf
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Queues are in state Error if the wan cable is not connected
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Queues are in state Error if the wan cable is not connected
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [VLAN][QOS][WNC] Changing the WANMode to vlan, QoS queues creating will fail
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Plugins not starting at boot
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] fix startup
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] errors when DHCPv6client does not start
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Update lower layer when creating new wanmodes
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] vlan not disabled when switching from vlan to untagged
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Startup after getting lowerlayer name
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): No dhcp v4 address on LAN

### Changes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Turn off import-dbg
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - Index of insertion too big
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] NTP server on wnc not reachable
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] create more unit tests for time-manager
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] BBF Time Manager Datamodel Evolutions: Time.Server.
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] BBF Time Manager Datamodel Evolutions: Time.Client.
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
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Correct dependencies
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): [amxrt] All amx plugins should start with the -D option
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): mod dmproxy wrong path translation when destination is a parameter in Device.
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] Runtime dependency on libqosnode is missing
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): amx/mod_sahtrace does not select dynamically stderr or syslog
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Dir path in odl file has one dash too much
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Add unit-tests
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): expose bridgetable
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [CI] Fix typo in dependencies
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

## Release proj_prpl_M3-2022_v1.3.2 - 2022-11-25(08:51:08 +0000)

### Other

- [tr181-upnp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-upnp): Add runtime dependency on miniupnp

## Release proj_prpl_M3-2022_v1.3.1 - 2022-11-21(12:21:52 +0000)

### Other

- [mod-httpaccess-lighttpd](https://gitlab.com/prpl-foundation/components/core/modules/mod-httpaccess-lighttpd): Opensource component
- [tr181-httpaccess](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-httpaccess): Opensource component
- [tr181-upnp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-upnp): Opensource component

## Release proj_prpl_M3-2022_v1.3.0 - 2022-11-21(07:51:57 +0000)

### New

- [mod-httpaccess-lighttpd](https://gitlab.com/soft.at.home/httpaccess/modules/mod_httpaccess_lighttpd): Component added
- [tr181-httpaccess](https://gitlab.com/soft.at.home/httpaccess/applications/tr181-httpaccess): Component added

## Release proj_prpl_M3-2022_v1.2.2 - 2022-11-18(16:38:55 +0000)

## Release proj_prpl_M3-2022_v1.2.1 - 2022-11-18(13:58:00 +0000)

### Changes

- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] NTP server on wnc not reachable
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] create more unit tests for time-manager
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] BBF Time Manager Datamodel Evolutions: Time.Server.
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time): [tr181-time] BBF Time Manager Datamodel Evolutions: Time.Client.

## Release proj_prpl_M3-2022_v1.2.0 - 2022-11-18(11:40:58 +0000)

### New

- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): [tr181-dnssd] add advertisement datamodel

### Fixes

- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): Issue : HOP-2199 [CDRouter][IPv4][VLAN] FAIL: mDNS lookup for prplOS.local failed
- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): [tr181-dnssd] add Documentation and README

### Other

- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): tr181-dnssd: mDNS service is not available over IPv6

## Release proj_prpl_M3-2022_v1.1.1 - 2022-11-18(08:26:12 +0000)

## Release proj_prpl_M3-2022_v1.1.0 - 2022-11-18(08:15:34 +0000)

### New

- [tr181-upnp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-upnp): Component added

## Release proj_prpl_M3-2022_v1.0.1 - 2022-11-17(20:13:54 +0000)

## Release proj_prpl_M3-2022_v1.0.0 - 2022-11-17(19:15:22 +0000)

### Removed

- [libqosmod](https://gitlab.com/prpl-foundation/components/core/libraries/libqosmod): Component removed

### New

- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [tr181-dhcpv6s] Interface status listening
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s): [prpl][amx][pcm][dhcpv6server] Definition of Upgrade Persistent DHCPv6 Server Configuration
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Implement the stats object
- [libqoscommon](https://gitlab.com/prpl-foundation/components/core/libraries/libqoscommon): Component added
- [libqosnode](https://gitlab.com/prpl-foundation/components/core/libraries/libqosnode): Component added
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [prpl][qos] Integrate new TR-181 parameters for Device.QoS v2.16
- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): Component added
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm): [PCM] PCM-Manager support restore on register and auto sync ctrl
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): Component added
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): Dynamic handling of network events (PPP)
- [tr181-dnssd](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dnssd): Component added
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): It must be possible to load additional iptables fragments files
- [tr181-logical](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-logical): Component added
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Issue:  HOP-1572 [tr181-ppp] Make module which configures ppp without netifd
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [PCM] [PPP] [upgrade persistency] Mark PPP Parameters as upgrade persistent
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Integrate new TR-181 parameters for Device.QoS v2.16
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Expand unit tests for node creation
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Integrate netmodel to translate interfaces
- [tr181-xpon](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-xpon): Component added
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
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip): Issues with dm functions not using internal structure
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
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] Error_Misconfigured Status when AssuredRate is unconfigured
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Valgrind complains about uninitialized values
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Should not pass NULL pointer to stat function
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Revert Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Failing transactions during stats read
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Remove overwriting interface status
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): No connection to lan after firstboot
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): PPP instances never come up
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): bad typecast
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Netdev instability when performing firstboots
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
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): support multiple servers of DHCP/ppp/router-advertisement
- [tr181-dns](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dns): default ODL configures "mod-dns-unbound" but "mod-dns-uci" (dnsmasq) is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): when bridge br-lan is down eth3 is used
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): after reboot default services are not loaded
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Index of insertion too big (ssh plugin)
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall): Add MSS rules for ppp interface traffic
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): [tr181-neighbordiscovery] allow icmpv6 packet on the firewall
- [tr181-neighbordiscovery](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-neighbordiscovery): Add fw rule faster
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): - [tr181-ppp] Use netmodel queries to find the linux interface
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] Datamodel in error while the HGW got an IP from the the PPP server
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): [tr181-ppp] fix installation path of direct module
- [tr181-ppp](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ppp): Buffer ppp script data in case the lowerlayer interface is still unknown
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): Enable core dumps by default
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos][Regression] Queue.TrafficClasses values unexpectedly overwritten
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Segmentation Error when trying to access QoS. datamodel
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Do not require on NetModel.Intf
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Queues are in state Error if the wan cable is not connected
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [QoS] Queues are in state Error if the wan cable is not connected
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [VLAN][QOS][WNC] Changing the WANMode to vlan, QoS queues creating will fail
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement): Plugins not starting at boot
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] fix startup
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing): [wan-autosensing] errors when DHCPv6client does not start
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] Update lower layer when creating new wanmodes
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): [WANManager] vlan not disabled when switching from vlan to untagged
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): Startup after getting lowerlayer name
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager): No dhcp v4 address on LAN

### Changes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Turn off import-dbg
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - Index of insertion too big
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
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Correct dependencies
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca): [amxrt] All amx plugins should start with the -D option
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): mod dmproxy wrong path translation when destination is a parameter in Device.
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] Runtime dependency on libqosnode is missing
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): Add functions to make the tracelevel and zones runtime configurable
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace): amx/mod_sahtrace does not select dynamically stderr or syslog
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): Dir path in odl file has one dash too much
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [amxrt] All amx plugins should start with the -D option
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Add unit-tests
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): expose bridgetable
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [CI] Fix typo in dependencies
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

## Release proj_prpl_M2-2022_v1.2.10 - 2022-11-04(08:55:39 +0000)

## Release proj_prpl_M2-2022_v1.2.9 - 2022-10-26(18:30:24 +0000)

## Release proj_prpl_M2-2022_v1.2.8 - 2022-10-25(09:54:25 +0000)

### Other

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): add wifi guest vaps
- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): : [pwhm] detect radios by context and not by pci order
- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): : [pwhm] detect radios by context and not by pci order
- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): [prpl] set prplOS as default SSIDs and disable them by default

## Release proj_prpl_M2-2022_v1.2.7 - 2022-10-24(13:06:17 +0000)

### Fixes

- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Netdev instability when performing firstboots

### Other

- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Add unit-tests

## Release proj_prpl_M2-2022_v1.2.6 - 2022-10-18(13:35:17 +0000)

### Fixes

- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): dm_info.c: fix typos in prpl field names

### Changes

- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): onu_hal_mock: support dm:object-changed for onu_activation
- [mod-xpon-prpl](https://gitlab.com/prpl-foundation/components/core/modules/mod-xpon-prpl): southbound_if.c: improve error message

### Other

- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): [SSHServer] Reduce log levels of some debug logs
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): [TR181-SSH] ssh instability when performing firstboots
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): Improve plugin boot order
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): [amx][ssh] Too many restarts when Enabling an Ssh instance
- [ssh-server](https://gitlab.com/prpl-foundation/components/core/plugins/ssh-server): [amx][ssh-server] Remove the Vendor Extension X_PRPL-COM_ from the SSH root object.

## Release proj_prpl_M2-2022_v1.2.5 - 2022-09-30(12:37:32 +0000)

### Fixes

- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Revert Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Issue HOP-1855: Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Route/Neigh/Addr not removed from datamodel when removed in Linux
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): bad typecast

### Other

- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): expose bridgetable
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): [CI] Fix typo in dependencies

## Release proj_prpl_M2-2022_v1.2.4 - 2022-09-21(06:36:54 +0000)

### Fixes

- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): Failing transactions during stats read
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): No connection to lan after firstboot
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev): PPP instances never come up

## Release proj_prpl_M2-2022_v1.2.3 - 2022-09-09(11:55:06 +0000)

## Release proj_prpl_M2-2022_v1.2.2 - 2022-09-09(09:06:25 +0000)

### Changes

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - Index of insertion too big

### Other

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Correct dependencies

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

