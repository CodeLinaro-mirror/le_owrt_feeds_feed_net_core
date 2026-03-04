# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.39.4)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=tr181-dhcpv6client
PKG_VERSION:=sah-next-4.1_v0.4.3
SHORT_DESCRIPTION:=TR-181 compatible DHCPv6 client

PKG_SOURCE:=tr181-dhcpv6client-sah-next-4.1_v0.4.3.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client/-/archive/sah-next-4.1_v0.4.3
PKG_HASH:=8df2e3b9270d228f25a26a828378099cda0ec92a46d0468816fdc7b0c8ac865b
PKG_BUILD_DIR:=$(BUILD_DIR)/tr181-dhcpv6client-sah-next-4.1_v0.4.3
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=tr181-dhcpv6client

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S25$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K75$(COMPONENT)
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=TR-181 Managers
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv6client
  DEPENDS += +libamxb
  DEPENDS += +libamxc
  DEPENDS += +libamxd
  DEPENDS += +libamxj
  DEPENDS += +libamxm
  DEPENDS += +libamxo
  DEPENDS += +libamxp
  DEPENDS += +amxrt
  DEPENDS += +libsahtrace
  DEPENDS += +libdhcpoptions
  DEPENDS += +libnetmodel
  DEPENDS += +mod-netmodel
  DEPENDS += +mod-dmext
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	TR-181 compatible DHCPv6 client
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_GROUP) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_SENTOPTION_17=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_SENTOPTION_17) CONFIG_GATEWAY=$(CONFIG_GATEWAY) CONFIG_ACCESSPOINT=$(CONFIG_ACCESSPOINT))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_GROUP) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_SENTOPTION_17=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_SENTOPTION_17) CONFIG_GATEWAY=$(CONFIG_GATEWAY) CONFIG_ACCESSPOINT=$(CONFIG_ACCESSPOINT))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(PKG_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(PKG_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_RUN_AS_GROUP) CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_SENTOPTION_17=$(CONFIG_SAH_AMX_TR181_DHCPV6CLIENT_SENTOPTION_17) CONFIG_GATEWAY=$(CONFIG_GATEWAY) CONFIG_ACCESSPOINT=$(CONFIG_ACCESSPOINT))
	$(call SAHInit/Install,$(STAGING_DIR))
endef

define Package/$(PKG_NAME)/install
	$(CP) $(PKG_INSTALL_DIR)/* $(1)/
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
