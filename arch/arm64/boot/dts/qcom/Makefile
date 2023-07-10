# SPDX-License-Identifier: GPL-2.0

ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
	dtbo-y += \
		sdm845-mtp-overlay.dtbo \
		sdm845-v2-mtp-overlay.dtbo \
		sdm845-v2.1-mtp-overlay.dtbo

	dtbo-$(CONFIG_MACH_XIAOMI_E5) += \
		xiaomi/perseus/perseus-p0-v2.1-overlay.dtbo \
		xiaomi/perseus/perseus-p1-v2.1-overlay.dtbo \
		xiaomi/perseus/perseus-p1_2-v2.1-overlay.dtbo \
		xiaomi/perseus/perseus-p2-v2.1-overlay.dtbo \
		xiaomi/perseus/perseus-p3-v2.1-overlay.dtbo \
		xiaomi/perseus/perseus-mp-v2.1-overlay.dtbo

sdm845-mtp-overlay.dtbo-base := sdm845.dtb
sdm845-v2-mtp-overlay.dtbo-base := sdm845-v2.dtb
sdm845-v2.1-mtp-overlay.dtbo-base := sdm845-v2.1.dtb

perseus-p0-v2.1-overlay.dtbo-base := sdm845-v2.1.dtb
perseus-p1-v2.1-overlay.dtbo-base := sdm845-v2.1.dtb
perseus-p1_2-v2.1-overlay.dtbo-base := sdm845-v2.1.dtb
perseus-p2-v2.1-overlay.dtbo-base := sdm845-v2.1.dtb
perseus-p3-v2.1-overlay.dtbo-base := sdm845-v2.1.dtb
perseus-mp-v2.1-overlay.dtbo-base := sdm845-v2.1.dtb
endif

dtb-$(CONFIG_ARCH_QCOM)	+= apq8016-sbc.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= apq8096-db820c.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= ipq8074-hk01.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8916-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8992-bullhead-rev-101.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8994-angler-rev-101.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= msm8996-mtp.dtb
dtb-$(CONFIG_ARCH_QCOM)	+= sdm845-mtp.dtb

dtb-$(CONFIG_MACH_XIAOMI_E10) := xiaomi/beryllium/beryllium-mp-v2.1.dtb
dtb-$(CONFIG_MACH_XIAOMI_E5) := \
	xiaomi/perseus/perseus-p0-v2.dtb \
	xiaomi/perseus/perseus-p0-v2.1.dtb \
	xiaomi/perseus/perseus-p1-v2.1.dtb \
	xiaomi/perseus/perseus-p1_2-v2.1.dtb \
	xiaomi/perseus/perseus-p2-v2.1.dtb \
	xiaomi/perseus/perseus-p3-v2.1.dtb \
	xiaomi/perseus/perseus-mp-v2.1.dtb

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
