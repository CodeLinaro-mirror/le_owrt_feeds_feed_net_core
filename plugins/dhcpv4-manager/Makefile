# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.40.6)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=dhcpv4-manager
RAW_VERSION:=sah-next-4.1_v4.0.2
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=Implementation of Device

PKG_SOURCE:=tr181-dhcpv4-sah-next-4.1_v4.0.2.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4/-/archive/sah-next-4.1_v4.0.2
PKG_HASH:=6bc8592d6ac48e3011a187ef6b09fa73ffe3c4e16b727f4a0cb32e40facaffd6
PKG_BUILD_DIR:=$(BUILD_DIR)/tr181-dhcpv4-sah-next-4.1_v4.0.2
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=dhcpv4-manager

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S40$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K60$(COMPONENT)
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=TR-181 Managers
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4
  DEPENDS += +amxrt
  DEPENDS += +libamxc
  DEPENDS += +libamxj
  DEPENDS += +libamxp
  DEPENDS += +libamxd
  DEPENDS += +libamxb
  DEPENDS += +libamxo
  DEPENDS += +libamxs
  DEPENDS += +libamxm
  DEPENDS += +libsahtrace
  DEPENDS += +libnetmodel
  DEPENDS += +mod-dmext
  DEPENDS += +mod-fw-amx
  DEPENDS += +libdhcpoptions
  DEPENDS += +rpcd
  DEPENDS += +ip-manager
  DEPENDS += +netmodel
  DEPENDS += +tr181-firewall
  DEPENDS += +time-manager
  DEPENDS += +dnsmasq-prpl
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	Implementation of Device.DHCPv4.Server object of the TR-181 datamodel
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_USER=$(CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_USER) CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_GROUP=$(CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_GROUP))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_USER=$(CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_USER) CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_GROUP=$(CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_GROUP))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_USER=$(CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_USER) CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_GROUP=$(CONFIG_SAH_SERVICES_AMX-DHCPV4-MANAGER_RUN_AS_GROUP))
	$(call SAHInit/Install,$(STAGING_DIR))
endef

define Package/$(PKG_NAME)/install
	if [ -d $(PKG_INSTALL_DIR) ]; then \
		$(CP) $(PKG_INSTALL_DIR)/* $(1)/; \
	fi
	if [ -d ./files ]; then \
		$(CP) ./files/* $(1)/; \
	fi
	find $(1) -name *.a -exec rm {} +;
	find $(1) -name *.h -exec rm {} +;
	find $(1) -name *.pc -exec rm {} +;
endef

define Package/$(PKG_NAME)/config
	source "$(SOURCE)/Config.in"
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
