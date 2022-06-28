# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]


## Release proj_prpl_v1.1.2 - 2022-06-28(07:00:49 +0000)

### Fixes

- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): Check if subscription exists
- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): [Gitlab CI][Unit tests][valgrind] Pipeline doesn't stop when memory leaks are detected

### Other

- [mod-dmproxy](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmproxy): mod dmproxy wrong path translation when destination is a parameter in Device.

## Release proj_prpl_v1.1.1 - 2022-06-14(14:07:15 +0000)

## Release proj_prpl_v1.1.0 - 2022-06-02(10:12:48 +0000)

### New

- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Add cwmp_plugin template and add port for cwmpd_conn_req in firewall

## Release proj_prpl_v1.0.3 - 2022-05-30(11:43:32 +0000)

## Release proj_prpl_v1.0.2 - 2022-05-30(11:39:53 +0000)

### Fixes

- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Set realistic shaping rates for the default configuration

## Release proj_prpl_v1.0.1 - 2022-05-18(09:21:48 +0000)

### Fixes

- [mod-dmext](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmext): [prpl][qos] After a save(), the QoS plugin does not start anymore
- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): - [mod-qos-tc] HTB shaping rate is set incorrectly
- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Update rate limits for tr181-qos

## Release proj_prpl_v1.0.0 - 2022-04-27(13:43:28 +0000)

### Breaking

- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): [Libfwrules] add mask to mark

### New

- [mod-qos-tc](https://gitlab.com/prpl-foundation/components/core/modules/mod-qos-tc): Component added
- [odl-generator](https://gitlab.com/prpl-foundation/components/utilities/odl-generator): Update templates to be compatible with tr181-qos v1.1.9

### Fixes

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): RAPlugin must configure the Firewall
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): [folder] Cleanup unused rules when invoking fw_folder_delete
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] QueueKey must be used as queue identifier

### Changes

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): Use BSD-2-Clause-Patent license
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): [GetDebugInformation] Add data model debuginfo in component services
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] move classificationkey to queuekey and add interface parameter to scheduler
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Rework variants for tc module
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [prpl][qos] Startup order does not work

### Other

- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - [libfwinterface] Document code
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): - [libfwinterface] Document code
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): move ClassificationKey to queues and add interface parameter to scheduler
- [libfwinterface](https://gitlab.com/prpl-foundation/components/core/libraries/libfwinterface): [CI] Fix BUILD_DEPS for debian bullseye
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): Use BSD-2-Clause-Patent license
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): - [libfwrules] Document code
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): - [libfwrules] Document code
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): Document code
- [libfwrules](https://gitlab.com/prpl-foundation/components/core/libraries/libfwrules): Change documentation path
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): Update documentation
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): Update documentation
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Document code
- [tr181-qos](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-qos): - [tr181-qos] Document code

## Release proj_prpl_v0.0.4 - 2022-03-29(09:02:58 +0000)

### Changes

- [mod-pcm-svc](https://gitlab.com/prpl-foundation/components/core/modules/mod-pcm-svc): Component downstepped from v0.3.0 to v0.2.1

## Release proj_prpl_v0.0.3 - 2022-03-29(07:49:17 +0000)

### Changes

- [deviceinfo-manager](https://gitlab.com/prpl-foundation/components/core/plugins/tr181-deviceinfo): Component downstepped from v1.2.2 to v1.0.3

## Release proj_prpl_v0.0.2 - 2022-03-28(15:14:22 +0000)

### Changes

- [mod-dmstats](https://gitlab.com/prpl-foundation/components/core/modules/mod-dmstats): Component downstepped from v0.2.1 to v0.1.1
- [mod-vlan-ioctl](https://gitlab.com/prpl-foundation/components/core/modules/mod-vlan-ioctl): Component downstepped from v1.0.3 to v0.1.1

## Release proj_prpl_v0.0.1 - 2022-03-28(14:59:19 +0000)

