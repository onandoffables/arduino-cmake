#====================================================================#
# Original blink sketch (from Arduino SDK examples)
#====================================================================#

# Some installations have renamed the example directories
if (EXISTS "${ARDUINO_SDK_PATH}/examples/01.Basics/Blink")
    set(BLINK_SKETCH "${ARDUINO_SDK_PATH}/examples/01.Basics/Blink")
else()
    set(BLINK_SKETCH "${ARDUINO_SDK_PATH}/examples/1.Basics/Blink")
endif()

generate_arduino_firmware(blink_original
    SKETCH "${BLINK_SKETCH}"
    PORT  /dev/ttyAMA0
    PROGRAMMER linuxgpio
    SERIAL minicom @SERIAL_PORT@)

# Alternative: by variables
#set(blink_original_SKETCH "${BLINK_SKETCH}")
#set(blink_original_PORT  /dev/ttyACM0)
#set(blink_original_SERIAL picocom @SERIAL_PORT@)
#set(blink_original_BOARD uno)
#
#generate_arduino_firmware(blink_original)
