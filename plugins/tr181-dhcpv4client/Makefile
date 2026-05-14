# WARNING: Automatically generated file using BAF (Build system Agnostic File) tooling (version 2.40.6)
# WARNING: You should contribute changes to https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client/-/blob/main/baf.yml instead
include $(TOPDIR)/rules.mk

PKG_NAME:=tr181-dhcpv4client
RAW_VERSION:=sah-next-4.1_v1.0.1
PKG_VERSION:=$(if $(filter v0% v1% v2% v3% v4% v5% v6% v7% v8% v9%,$(RAW_VERSION)),$(patsubst v%,%,$(RAW_VERSION)),$(RAW_VERSION))
SHORT_DESCRIPTION:=TR-181 compatible DHCPv4 client

PKG_SOURCE:=tr181-dhcpv4client-sah-next-4.1_v1.0.1.tar.gz
PKG_SOURCE_URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client/-/archive/sah-next-4.1_v1.0.1
PKG_HASH:=d4078e07cbf3e03ea7e9522c59b87497308a3b7042de38b75c5f2ee81d59e908
PKG_BUILD_DIR:=$(BUILD_DIR)/tr181-dhcpv4client-sah-next-4.1_v1.0.1
PKG_MAINTAINER:=Soft At Home <support.opensource@softathome.com>
PKG_LICENSE:=BSD-2-Clause-Patent
PKG_LICENSE_FILES:=LICENSE

COMPONENT:=tr181-dhcpv4client

PKG_RELEASE:=1

define SAHInit/Install
	install -d $(1)/etc/rc.d/
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/S27$(COMPONENT)
	ln -sfr $(1)/etc/init.d/$(COMPONENT) $(1)/etc/rc.d/K75$(COMPONENT)
endef

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
  CATEGORY:=prpl Foundation
  SUBMENU:=TR-181 Managers
  TITLE:=$(SHORT_DESCRIPTION)
  URL:=https://gitlab.com/prpl-foundation/components/core/plugins/tr181-dhcpv4client
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
  DEPENDS += +rpcd
  MENU:=1
endef

define Package/$(PKG_NAME)/description
	TR-181 compatible DHCPv4 client
endef

define Build/Compile
	$(call Build/Compile/Default, STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PKG_CONFIG_PATH=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_GROUP) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_SENTOPTION_125=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_SENTOPTION_125))
endef

define Build/Install
	$(call Build/Install/Default, install INSTALL=install D=$(PKG_INSTALL_DIR) DEST=$(PKG_INSTALL_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_GROUP) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_SENTOPTION_125=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_SENTOPTION_125))

	$(call SAHInit/Install,$(PKG_INSTALL_DIR))
endef

define Build/InstallDev
	$(call Build/Install/Default, install INSTALL=install D=$(STAGING_DIR) DEST=$(STAGING_DIR) STAGINGDIR=$(STAGING_DIR) CONFIGDIR=$(STAGING_DIR) PV=$(RAW_VERSION) PKG_CONFIG_LIBDIR=$(STAGING_DIR)/usr/lib/pkgconfig LIBDIR=/usr/lib INSTALL_LIB_DIR=/lib INSTALL_BIN_DIR=/bin RAW_VERSION=$(RAW_VERSION) HARDCO_HAL_DIR=$(STAGING_DIR)/usr/include PKG_CONFIG=$(PKG_CONFIG) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_USER=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_USER) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_GROUP=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_RUN_AS_GROUP) CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_SENTOPTION_125=$(CONFIG_SAH_AMX_TR181_DHCPV4CLIENT_SENTOPTION_125))
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
