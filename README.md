# Feed_net_core

SoftAtHome feed of Openwrt packages for networking components.

## Included components

Feed_net_core includes the following components:

### Libraries

- [libdhcpoptions](https://gitlab.com/soft.at.home/libraries/libdhcpoptions) - Library to parse and evaluate the binary data of DHCP options
- [libfwinterface](https://gitlab.com/soft.at.home/libraries/libfwinterface) - A library providing interfaces between lib_fwrules and netfilter
- [libfwrules](https://gitlab.com/soft.at.home/libraries/libfwrules) - A library to store ordered firewall rules
- [libnetmodel](https://gitlab.com/soft.at.home/libraries/libnetmodel) - NetModel client library

### Modules

- [mod-dmext](https://gitlab.com/soft.at.home/ambiorix/modules/mod-dmext) - Data model extension module

### Plugins

- [deviceinfo-manager](https://gitlab.com/soft.at.home/plugins/tr181-deviceinfo) - TR-181 compatible DeviceInfo plugin
- [dhcpv4-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv4) - Implementation of Device.DHCPv4 object of the TR-181 datamodel
- [dhcpv6s-manager](https://gitlab.com/soft.at.home/plugins/tr181-dhcpv6s) - Implementation of Device.DHCPv6.Server. object of the TR-181 datamodel
- [ip-manager](https://gitlab.com/soft.at.home/plugins/tr181-ip) - Implementation of Device.IP of the TR-181 datamodel
- [netdev-plugin](https://gitlab.com/soft.at.home/plugins/netdev) - NetDev monitors the operating system's network devices
- [netmodel](https://gitlab.com/soft.at.home/plugins/netmodel) - Network Model plugin
- [routing-manager](https://gitlab.com/soft.at.home/plugins/tr181-routing) - Implementation of Device.Routing of the TR-181 datamodel
- [time-manager](https://gitlab.com/soft.at.home/plugins/tr181-time) - TR181 Time plugin
- [tr181-bridging](https://gitlab.com/soft.at.home/plugins/tr181-bridging) - Implementation of Device.Bridging of the TR-181 datamodel
- [tr181-firewall](https://gitlab.com/soft.at.home/plugins/tr181-firewall) - TR181 firewall manager
- [wan-manager](https://gitlab.com/soft.at.home/plugins/wan-manager) - WAN Manager

### Other

These components are not managed by SoftAtHome.

- tr181-device

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
