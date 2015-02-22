# This configuration file outlines some of the ways Arduino CMake
# can be used. For a detailed explanation of all the options please
# reade README.rst.

#set(ARDUINO_DEFAULT_BOARD diecimila) # Default Board ID, when not specified
#set(ARDUINO_DEFAULT_PORT /dev/ttyUSB0) # Default Port, when not specified
set(ARDUINO_DEFAULT_BOARD avrpi8) # Default Board ID, when not specified
set(ARDUINO_DEFAULT_PORT /dev/ttyAMA0) # Default Port, when not specified

add_subdirectory(blink_original)
add_subdirectory(blink_bundled)
add_subdirectory(wire_example)
add_subdirectory(blink_lib)
add_subdirectory(AnalogInOutSerial)
add_subdirectory(keyboard)
