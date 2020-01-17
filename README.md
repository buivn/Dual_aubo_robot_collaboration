# Dual I5 AUBO Robot\ 

To run two I5 Aubo Robot simutalneously, two code files are changeds: \
- aubo_driver.h and aubo_driver.cpp (aubo_driver): adding a new constructor for AuboRobot class, which receive one more argument for the name of each robot. \

Adding two files to control two robots in folder (aubo_driver/src): \
- dual_controller.cpp: create a node which publishc a target_topic (six joints' angles) for both robots. \
- dual_robots.cpp: create two robot class/drivers which subcribed the target_topic and control the two robots moving to the new targets.







