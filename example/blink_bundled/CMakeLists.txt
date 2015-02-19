#====================================================================#
# Bundled blink sketch example
#====================================================================#
generate_arduino_firmware(blink_bundled
    SKETCH Blink
    PROGRAMMER linuxgpio
    NO_AUTOLIBS
    PORT  /dev/ttyAMA0
    SERIAL minicom @SERIAL_PORT@)

# Alternative: by variables
#set(blink_bundled_SKETCH Blink)
#set(blink_bundled_PROGRAMMER linuxgpio)
#set(blink_bundled_NO_AUTOLIBS true)
#
#generate_arduino_firmware(blink_bundled)
