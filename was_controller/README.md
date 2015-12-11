# was_controller

- Platform: ARMv7
- ROS Nodes: (total = 1)
	+ was_controller: receive commands from was_master, directly control actuators/motors via GPIO/UART
		> Subscribe:
			- lift_sub: Ultrasonic range sensors
				+ type 		: std_msgs::String
				+ topic		: "was_control/lift"
				+ callback 	: lift_cb