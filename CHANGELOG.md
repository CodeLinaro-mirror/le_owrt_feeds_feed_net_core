# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


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

