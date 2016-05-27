include $(TOPDIR)/rules.mk

PKG_NAME:=fff-openvpn
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/fff-openvpn

include $(INCLUDE_DIR)/package.mk

define Package/fff-openvpn
    SECTION:=base
    CATEGORY:=Freifunk
    TITLE:=Freifunk-Franken openvpn configuration script
    URL:=http://www.freifunk-franken.de
    DEPENDS:=+openvpn-mbedtls
endef

define Package/fff-openvpn/description
    This is the openvpn package for the Freifunk Franken Firmware
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

define Package/fff-openvpn/install
    # $(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,fff-openvpn))
