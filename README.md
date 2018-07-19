# ada_launch



## Launching the robot (default setup)

Simply run `roslaunch ada_launch default.launch`.

Next, you can run a demo from `ada_demos`, that uses the plain Ada robot without any attachments.

## Launching the robot for the feeding demo

The feeding demo requires some more configuration and some additional nodes.
It can be started by running `roslaunch ada_launch default.launch feeding:=true`.

You may also need to start
- The camera node, running directly on the camera board. Typically the script is called something like `run_all.sh`
- The forque sensor controller, using `roslaunch forque_sensor_hardware forque.launch`
- The feeding demo parameters, and the feeding demo itself.
