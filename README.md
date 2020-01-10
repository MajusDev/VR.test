# VR.test

This the page for my simple VR test using Godot and GDScript

It will only be supporting Rift headsets for now until i make a vive/openvr compatable one

When it is done I will push it here 

# Bug reports will come soon (when I get to it)

Bug report 1/9/20
Following function did not work as intended

func _ready():

	interface = ARVRServer.find_interface("Openvr")
	
	if interface and interface.initialize():

had to replace with 

func _ready():

	interface = ARVRServer.find_interface("Oculus")
	
	if interface and interface.initialize():
  
to work with my Oculus Rift S
