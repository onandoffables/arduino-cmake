#====================================================================#
# Advanced static library example
#====================================================================#
generate_arduino_library(blink_lib
    SRCS blink_lib.cpp
    HDRS blink_lib.h)

# Alternative: by variables
#set(blink_lib_SRCS blink_lib.cpp)
#set(blink_lib_HDRS blink_lib.h)
#set(blink_lib_BOARD uno)
#
#generate_arduino_library(blink_lib)

#====================================================================#
# Advanced firmware example
#====================================================================#

generate_arduino_firmware(blink
    SRCS blink.cpp
    LIBS blink_lib
    PROGRAMMER linuxgpio)

# Alternative: by variables
#set(blink_SRCS blink.cpp)
#set(blink_LIBS blink_lib)
#set(blink_BOARD uno)
#
#generate_arduino_firmware(blink)
