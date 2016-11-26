###############################################################################
# Project Name: based on Project Path and used to define OSEK configuration file
PROJECT_NAME               = $(lastword $(subst $(DS), , $(PROJECT_PATH)))
# Project path
# Defined $(PROJECT_PATH) in makefile.mine
# source path
$(PROJECT_NAME)_SRC_PATH  += $(PROJECT_PATH)$(DS)src
# include path
INC_FILES            += $(PROJECT_PATH)$(DS)inc
# library source files
SRC_FILES            += $(wildcard $($(PROJECT_NAME)_SRC_PATH)$(DS)*.c)
# configuration for OSEK-OS
OIL_FILES            += $(PROJECT_PATH)$(DS)etc$(DS)$(PROJECT_NAME).oil
# Modules needed for this example
MODS ?= modules$(DS)posix           \
        modules$(DS)ciaak           \
        modules$(DS)drivers         \
        modules$(DS)rtos            \
        modules$(DS)libs

