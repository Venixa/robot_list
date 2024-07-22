# robot_list
List the robot tests by taking robot flags as cmd line arguments </br>

Usage: </br>
python -m robot_list.robot_list '--include test1 --exclude test2 tests/' </br>
python -m robot_list.robot_list '-i test1 -e test2 tests/' </br>
python -m robot_list.robot_list '--suite suite1 --test test1 tests/'  </br>
python -m robot_list.robot_list '-s suite1 -t test1 tests/' </br>
python -m robot_list.robot_list '--include test1 --exclude test2 --suite suite1 tests/' </br>
python -m robot_list.robot_list '-i test1 -e test2 -s suite1 tests/' </br>
 </br>
or </br> </br>

from robot_list import robot_list
robot_list = robot_list.RobotList(command) </br>
test_dict, test_list = robot_list.list_robot_tests() </br>

If --suite is provided within the argument then it test_dict will be populated otherwise test_list will only be populated
