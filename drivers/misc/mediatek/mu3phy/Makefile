include $(srctree)/drivers/misc/mediatek/Makefile.custom

ifeq ($(CONFIG_USB_DEBUG),y)
	EXTRA_CFLAGS += -DDEBUG
endif
obj-$(CONFIG_MU3_PHY) := mu3phy.o

mu3phy-$(CONFIG_MU3_PHY) := mtk-phy.o
mu3phy-$(CONFIG_U3_PHY_GPIO_SUPPORT) += mtk-phy-gpio.o
mu3phy-$(CONFIG_U3_PHY_AHB_SUPPORT) += mtk-phy-ahb.o
mu3phy-$(CONFIG_C60802_SUPPORT) += mtk-phy-c60802.o
mu3phy-$(CONFIG_D60802_SUPPORT) += mtk-phy-d60802.o
mu3phy-$(CONFIG_E60802_SUPPORT) += mtk-phy-e60802.o
mu3phy-$(CONFIG_A60810_SUPPORT) += mtk-phy-a60810.o


obj-$(CONFIG_MU3_PHY) += $(subst ",,$(CONFIG_MTK_PLATFORM))/

