include $(TOPDIR)/rules.mk

PKG_NAME:=fff-batman-adv-server
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/fff-batman-adv-server

include $(INCLUDE_DIR)/package.mk

define Package/fff-batman-adv-server
    SECTION:=base
    CATEGORY:=Freifunk
    TITLE:=Freifunk-Franken batman-adv-server
    URL:=http://www.freifunk-franken.de
    DEPENDS:=+fff-batman-adv
endef

define Package/fff-batman-adv-server/description
    This is the batman-adv-server for the Freifunk Franken Firmware
    It is used to re-configure batman-adv package as used in a server.
endef

define Build/Prepare
    echo "all: " > $(PKG_BUILD_DIR)/Makefile
endef

define Build/Configure
    # nothing
endef

define Build/Compile
    # nothing
endef

define Package/fff-batman-adv-server/install
    $(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,fff-batman-adv-server))
