ifneq ($(filter m y,$(CONFIG_INPUT_NOVA_0FLASH_MMI_ENABLE_DOUBLE_TAP)),)
	ccflags-y += -DNVT_SENSOR_EN
endif
ifneq ($(filter m y,$(CONFIG_INPUT_NOVA_PANEL_NOTIFICATIONS)),)
	ccflags-y += -DNVT_CONFIG_PANEL_NOTIFICATIONS
endif
ifneq ($(filter m y,$(CONFIG_INPUT_NOVA_PANEL_ESD_ENABLE)),)
	ccflags-y += -DNVT_ESD_ENABLE
endif

nova_0flash_mmi-y += nt36xxx.o
nova_0flash_mmi-y += nt36xxx_ext_proc.o
nova_0flash_mmi-y += nt36xxx_fw_update.o
nova_0flash_mmi-y += nt36xxx_mp_ctrlram.o

obj-$(CONFIG_TOUCHSCREEN_NT36xxx_HOSTDL_SPI_MMI) += nova_0flash_mmi.o
