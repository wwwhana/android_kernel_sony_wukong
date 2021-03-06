obj-y += io.o dma.o memory.o
ifndef CONFIG_ARM_ARCH_TIMER
obj-y += timer.o
endif
obj-$(CONFIG_USE_OF) += board-dt.o

obj-y += acpuclock.o
obj-$(CONFIG_HW_PERF_EVENTS) += perf_trace_counters.o perf_trace_user.o
obj-$(CONFIG_ARCH_MSM_KRAIT) += msm-krait-l2-accessors.o perf_event_msm_krait_l2.o
obj-$(CONFIG_ARCH_MSM_KRAIT) += krait-scm.o
obj-$(CONFIG_DEBUG_FS) += perf_debug.o

obj-$(CONFIG_SMP) += headsmp.o platsmp.o
obj-$(CONFIG_HOTPLUG_CPU) += hotplug.o

obj-$(CONFIG_MSM_TEST_QMI_CLIENT) += kernel_test_service_v01.o test_qmi_client.o

obj-$(CONFIG_MSM_PCIE) += pcie.o pcie_irq.o pcie_phy.o

obj-$(CONFIG_MSM_DMA_TEST) += dma_test.o
obj-$(CONFIG_SURF_FFA_GPIO_KEYPAD) += keypad-surf-ffa.o

obj-$(CONFIG_ARCH_FSM9900) += board-fsm9900.o board-fsm9900-gpiomux.o
obj-$(CONFIG_ARCH_FSM9900) += clock-fsm9900.o
obj-$(CONFIG_ARCH_FSM9900) += rfic-fsm9900.o bbif-fsm9900.o
obj-$(CONFIG_ARCH_FSM9010) += board-fsm9010.o
obj-$(CONFIG_QPNP_BMS) += bms-batterydata.o bms-batterydata-desay.o
obj-$(CONFIG_QPNP_BMS) += bms-batterydata-qrd-4v35-2000mah.o bms-batterydata-qrd-4v2-1300mah.o
obj-$(CONFIG_ARCH_APQ8084) += board-8084.o board-8084-gpiomux.o
obj-$(CONFIG_ARCH_APQ8084) += clock-8084.o clock-mdss-8974.o
obj-$(CONFIG_ARCH_MSM8974) += board-8974.o
obj-$(CONFIG_ARCH_MSM8974) += clock-rpm-8974.o clock-gcc-8974.o clock-mmss-8974.o clock-lpass-8974.o clock-mdss-8974.o
obj-$(CONFIG_KRAIT_REGULATOR) += krait-regulator.o  krait-regulator-pmic.o
obj-$(CONFIG_ARCH_MDM9630) += board-9630.o board-9630-gpiomux.o
obj-$(CONFIG_MSM_PP2S_FEMTO) += pp2s.o
obj-$(CONFIG_ARCH_MSM8909) += board-8909.o
obj-$(CONFIG_ARCH_MSM8916) += board-8916.o
obj-$(CONFIG_ARCH_MSM8226) += board-8226.o 
obj-$(CONFIG_ARCH_MSM8226) += clock-8226.o clock-mdss-8974.o
obj-$(CONFIG_ARCH_MSM8610) += board-8610.o board-8610-gpiomux.o
obj-$(CONFIG_ARCH_MSM8610) += clock-8610.o
obj-$(CONFIG_ARCH_MSM8610) += clock-dsi-8610.o
obj-$(CONFIG_ARCH_MDM9630) += clock-9630.o
obj-$(CONFIG_ARCH_MSMZIRC) += board-zirc.o
obj-$(CONFIG_ARCH_MDMFERRUM) += board-8909.o
obj-$(CONFIG_MSM_PM) += ext-buck-control.o

ifdef CONFIG_MACH_SONY_FLAMINGO
	obj-$(CONFIG_MACH_SONY_FLAMINGO) += board-sony_yukon_flamingo-gpiomux.o bms-batterydata-flamingo.o
else ifdef CONFIG_MACH_SONY_EAGLE
        obj-$(CONFIG_MACH_SONY_EAGLE) += board-sony_yukon_eagle-gpiomux.o bms-batterydata-eagle.o
else ifdef CONFIG_MACH_SONY_TIANCHI
	obj-$(CONFIG_MACH_SONY_TIANCHI) += board-sony_yukon_tianchi-gpiomux.o bms-batterydata-tianchi.o
else ifdef CONFIG_MACH_SONY_WUKONG
	obj-$(CONFIG_MACH_SONY_WUKONG) += board-sony_yukon_wukong-gpiomux.o bms-batterydata-wukong.o
else ifdef CONFIG_MACH_SONY_SEAGULL
	obj-$(CONFIG_MACH_SONY_SEAGULL) += board-sony_yukon_seagull-gpiomux.o bms-batterydata-seagull.o
else
	obj-$(CONFIG_ARCH_MSM8226) += board-8226-gpiomux.o bms-batterydata-oem.o
endif

obj-$(CONFIG_MACH_SONY_YUKON) += board-sony_yukon-nfc.o

ifdef CONFIG_MACH_SONY_SIRIUS
	obj-$(CONFIG_MACH_SONY_SIRIUS) += board-sony_shinano_sirius-gpiomux.o bms-batterydata-sirius.o
else ifdef CONFIG_MACH_SONY_CASTOR
	obj-$(CONFIG_MACH_SONY_CASTOR) += board-sony_shinano_castor-gpiomux.o bms-batterydata-castor.o
else ifdef CONFIG_MACH_SONY_LEO
	obj-$(CONFIG_MACH_SONY_LEO) += board-sony_shinano_leo-gpiomux.o bms-batterydata-leo.o
else ifdef CONFIG_MACH_SONY_ARIES
	obj-$(CONFIG_MACH_SONY_ARIES) += board-sony_shinano_aries-gpiomux.o bms-batterydata-aries.o
else ifdef CONFIG_MACH_SONY_SCORPION
	obj-$(CONFIG_MACH_SONY_SCORPION) += board-sony_shinano_scorpion-gpiomux.o bms-batterydata-scorpion.o
else ifdef CONFIG_MACH_SONY_TOGARI_ROW
	obj-$(CONFIG_MACH_SONY_TOGARI_ROW) += board-sony_rhine_togari_row-gpiomux.o bms-batterydata-togari.o
else ifdef CONFIG_MACH_SONY_HONAMI_ROW
	obj-$(CONFIG_MACH_SONY_HONAMI_ROW) += board-sony_rhine_honami_row-gpiomux.o bms-batterydata-honami.o
else ifdef CONFIG_MACH_SONY_AMAMI_ROW
	obj-$(CONFIG_MACH_SONY_AMAMI_ROW) += board-sony_rhine_amami_row-gpiomux.o bms-batterydata-amami.o
else
	obj-$(CONFIG_ARCH_MSM8974) += board-8974-gpiomux.o bms-batterydata-oem.o
endif

obj-$(CONFIG_MACH_SONY_SHINANO) += board-sony_shinano-gpiomux-ref.o board-sony_shinano-nfc.o
obj-$(CONFIG_MACH_SONY_RHINE) += board-sony_rhine-gpiomux-ref.o
obj-$(CONFIG_ARCH_MSM8974) += sony_gpiomux.o

CFLAGS_msm_vibrator.o += -Idrivers/staging/android

obj-$(CONFIG_MSM_LPM_TEST) += test-lpm.o


obj-$(CONFIG_ARCH_MSM8974) += gpiomux-v2.o gpiomux.o
obj-$(CONFIG_ARCH_MDM9630) += gpiomux-v2.o gpiomux.o
obj-$(CONFIG_ARCH_MSM8226) += gpiomux-v2.o gpiomux.o
obj-$(CONFIG_ARCH_MSM8610) += gpiomux-v2.o gpiomux.o
obj-$(CONFIG_ARCH_APQ8084) += gpiomux-v2.o gpiomux.o
obj-$(CONFIG_ARCH_FSM9900) += gpiomux-v2.o gpiomux.o

obj-$(CONFIG_MSM_CACHE_ERP) += cache_erp.o

obj-$(CONFIG_MSM_HSIC_SYSMON) += hsic_sysmon.o
obj-$(CONFIG_MSM_HSIC_SYSMON_TEST) += hsic_sysmon_test.o

obj-$(CONFIG_MSM_RPC_USB) += rpc_hsusb.o rpc_fsusb.o

obj-$(CONFIG_MEMORY_HOLE_CARVEOUT) +=  msm_mem_hole.o

obj-$(CONFIG_MSM_SMCMOD) += smcmod.o

obj-$(CONFIG_ARCH_MSM8974) += msm_mpmctr.o

obj-$(CONFIG_PERFMAP) += perfmap.o

obj-$(CONFIG_HAS_MACH_MEMUTILS) += memutils/
