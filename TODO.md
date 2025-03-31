Split current code into 3 tasks

-Initialize Task
	Has the highest priority and runs first, initializes the ethernet communications
-Telemetry Task
	Has the second highest priority, send telemetry then suspends itself for a second
-Main Loop
	Handles the rest of the stuff. When an image request is received, suspends the telemetry task


 Helper Functions
 -getTelemetry
 	Grabs telemetry data from relevant GPIO pins
  
