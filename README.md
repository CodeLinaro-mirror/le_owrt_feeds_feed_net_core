# Feed_net_core

SoftAtHome feed of Openwrt packages for networking components.

## Included components

Feed_net_core includes the following components:

### Libraries

- [libdhcpoptions](https://gitlab.com/prpl-foundation/components/core/libraries/libdhcpoptions) - Library to parse and evaluate the binary data of DHCP options
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface) - A library providing interfaces between libfwrules and netfilter
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules) - A library to store ordered firewall rules
- [libnetmodel](https://gitlab.com/prpl-foundation/components/core/libraries/libnetmodel) - NetModel client library

### Modules

- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext) - Data model extension module
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy) - Data model object proxy
- [mod-dmstats](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmstats) - Reusable stats module
- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc) - Upgrade Persistent Configuration Manager service module
- [mod-sahtrace](https://gitlab.com/prpl-foundation/components/core/modules/mod-sahtrace) - Module for sahtrace logging
- [mod-vlan-ioctl](https://gitlab.com/prpl-foundation/components/core/modules/mod-vlan-ioctl) - SoC module to help handling vlans
- [mod-vlan-uci](https://gitlab.com/prpl-foundation/components/core/modules/mod-vlan-uci) - SoC module to help handling vlans

### Plugins

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo) - TR-181 compatible DeviceInfo plugin
- [dhcpv4-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4) - Implementation of Device.DHCPv4 object of the TR-181 datamodel
- [dhcpv6s-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6s) - Implementation of Device.DHCPv6.Server. object of the TR-181 datamodel
- [ethernet-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ethernet) - Ethernet plugin
- [ip-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-ip) - Implementation of Device.IP of the TR-181 datamodel
- [moca-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-moca) - moca plugin
- [multisettings](https://gitlab.com/prpl-foundation/components/core/plugins/multisettings) - multisettings plugin
- [netdev-plugin](https://gitlab.com/prpl-foundation/components/core/plugins/netdev) - NetDev monitors the operating system's network devices
- [netmodel](https://gitlab.com/prpl-foundation/components/core/plugins/netmodel) - Network Model plugin
- [pcm-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-pcm) - Upgrade Persistent Configuration Manager
- [routing-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routing) - Implementation of Device.Routing of the TR-181 datamodel
- [time-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-time) - TR181 Time plugin
- [tr181-bridging](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-bridging) - Implementation of Device.Bridging of the TR-181 datamodel
- [tr181-device](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-device) - TR-181 compatible Device plugin
- [tr181-dhcpv4client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client) - TR-181 compatible DHCPv4 client
- [tr181-dhcpv6client](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client) - TR-181 compatible DHCPv6 client
- [tr181-firewall](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-firewall) - TR181 firewall manager
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos) - TR-181 QoS model plugin
- [tr181-routeradvertisement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-routeradvertisement) - Implementation of Device.RouterAdvertisement object of the TR-181 datamodel
- [tr181-usermanagement](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-usermanagement) - tr181 user management plugin
- [wan-autosensing](https://gitlab.com/prpl-foundation/components/core/plugins/wan-autosensing) - WAN Autosensing
- [wan-manager](https://gitlab.com/prpl-foundation/components/core/plugins/wan-manager) - TR-181 compatible plugin for advanced WAN mode configuration

### Utilities

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator) - Odl generator using ucode.

## How to add feed_net_core to your OpenWrt build

At the root of your OpenWrt tree, add the following to your `feeds.conf` file:

```sh
src-git feed_net_core git@gitlab.com:soft.at.home/buildsystems/openwrt/feed_net_core.git;main
```

Add the packages to your OpenWrt instance with the following commands:
```sh
./scripts/feeds update feed_net_core #retrieve the feed from service/update to latest
./scripts/feeds install -p feed_net_core #make all of the feed packages available to the build
```
