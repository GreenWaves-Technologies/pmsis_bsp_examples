APP = test
SRCS += test.c
CFLAGS += -O3 -g
USE_PMSIS_BSP=1

RUNNER_CONFIG = $(CURDIR)/config.ini

BOARD ?= gapuino

ifeq '$(BOARD)' 'gapuino'
CFLAGS = -DGAPUINO -DHIMAX
endif

ifeq '$(BOARD)' 'gapoc_a'
CFLAGS = -DGAPOC_A -DUSE_BRIDGE
endif

include $(PULP_SDK_HOME)/install/rules/pmsis.mk
