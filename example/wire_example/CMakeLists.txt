#====================================================================#
# master_writer example from Wire library
#====================================================================#
generate_arduino_example(wire_example
                         LIBRARY Wire
                         EXAMPLE master_writer
                         PROGRAMMER linuxgpio)

# Alternative: by variables
#set(wire_example_LIBRARY Wire)
#set(wire_example_EXAMPLE master_writer)
#
#generate_arduino_example(wire_example)
