# SPDX-License-Identifier: GPL-2.0
#
# Makefile for the input core drivers.
#

# Each configuration option enables a list of files.

obj-$(CONFIG_INPUT)		+= input-core.o
input-core-y := input.o input-compat.o input-mt.o input-poller.o ff-core.o

obj-$(CONFIG_INPUT_FF_MEMLESS)	+= ff-memless.o
obj-$(CONFIG_INPUT_POLLDEV)	+= input-polldev.o
obj-$(CONFIG_INPUT_SPARSEKMAP)	+= sparse-keymap.o
obj-$(CONFIG_INPUT_MATRIXKMAP)	+= matrix-keymap.o

obj-$(CONFIG_INPUT_LEDS)	+= input-leds.o
obj-$(CONFIG_INPUT_MOUSEDEV)	+= mousedev.o
obj-$(CONFIG_INPUT_JOYDEV)	+= joydev.o
obj-$(CONFIG_INPUT_EVDEV)	+= evdev.o
obj-$(CONFIG_INPUT_EVBUG)	+= evbug.o

obj-$(CONFIG_INPUT_KEYBOARD)	+= keyboard/
obj-$(CONFIG_INPUT_MOUSE)	+= mouse/
obj-$(CONFIG_INPUT_JOYSTICK)	+= joystick/
obj-$(CONFIG_INPUT_TABLET)	+= tablet/
obj-$(CONFIG_INPUT_TOUCHSCREEN)	+= touchscreen/
obj-$(CONFIG_INPUT_MISC)	+= misc/

obj-$(CONFIG_INPUT_APMPOWER)	+= apm-power.o

obj-$(CONFIG_RMI4_CORE)		+= rmi4/
obj-$(CONFIG_INPUT_FINGERPRINT) += fingerprint/
obj-$(CONFIG_STMVL53L5)		+= stmvl53l5/

ifeq ($(TARGET_PRODUCT), diting)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_DITING
endif

ifeq ($(TARGET_PRODUCT), mayfly)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_MAYFLY
    KBUILD_CPPFLAGS += -DQCOM_HAPTIC_F0_PROTECT
endif

ifeq ($(TARGET_PRODUCT), zizhan)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_ZIZHAN
    KBUILD_CPPFLAGS += -DQCOM_HAPTIC_F0_PROTECT
endif

ifeq ($(TARGET_PRODUCT), mondrian)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_MONDRIAN
endif

ifeq ($(TARGET_PRODUCT), marble)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_MARBLE
    KBUILD_CPPFLAGS += -DQCOM_HAPTIC_F0_PROTECT
endif

ifeq ($(TARGET_PRODUCT), yudi)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_YUDI
    KBUILD_CPPFLAGS += -DQCOM_HAPTIC_F0_PROTECT
endif

ifeq ($(TARGET_PRODUCT), garnet)
    KBUILD_CPPFLAGS += -DCONFIG_TARGET_PRODUCT_GARNET
    KBUILD_CPPFLAGS += -DQCOM_HAPTIC_F0_PROTECT
endif
