# robot_list
List the robot tests by taking robot flags are command as cmd line arguments

Usage:
python -m robot_list '--include test1 --exclude test2 tests/'
python -m robot_list '-i test1 -e test2 tests/'
python -m robot_list '--suite suite1 --test test1 tests/'
python -m robot_list '-s suite1 -t test1 tests/'
python -m robot_list '--include test1 --exclude test2 --suite suite1 tests/'
python -m robot_list '-i test1 -e test2 -s suite1 tests/'

or

robot_list = RobotList(command)
robot_list.list_robot_tests()
