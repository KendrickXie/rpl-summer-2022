# Kendrick Xie

**Project name:** Locobot and OT2 Integration
**Advisor:** Rafael Vescovi / Ian Foster
**Email:** kxie@anl.gov

## Project description

## Diary

### 07/05

- Work on orientation requirements
- Tour lab

### 07/06

- Finish orientation requirements
- Read through RPL software/network brainstorm
- Work on [CV](https://github.com/KendrickXie/rpl-summer-2022/blob/main/kendrick/KendrickXieCV.pdf) through Overleaf and GitHub webpage

### 07/07

- Finished [webpage](https://kendrickxie.github.io)
- Attend GitHub tutorial meeting

### 07/08

- Attend weekly update meeting
- Take picture for personal and RPL webpages
- Complete required training for badge to access lab room

### 07/11

- Learn about funcx and Gladier and run examples
- Ran into problems with Gladier examples

### 07/12

- Troubleshoot Gladier examples and find that there is a problem with filepaths (maybe to due with Windows compatibility)
- Found problem with index insertion as well
- Attend Globus Labs meeting

### 07/13

- Learn about functionalities of OT-2 and LoCoBot

### 07/14

- Set up environment and learn how to run simulations for OT-2 and LoCoBot

### 07/15

- Set up WSL2
- Try running Gladier examples on WSL2, but ran into problem with only being allowed to deploy one flow

### 07/18

- Look at examples of protocols on OT-2s
- Research remote functionalities of LoCoBot

### 07/19

- Visit room with robots at UChicago and get key card access
- Attend Globus Labs meeting
- Connect to OT-2s and LoCoBot for the first time

### 07/20

- Updated one of the OT-2s and try and tried to use HTTP api but documentation is outdated
- Setup remote connection from laptop to LoCoBot with WSL2 and get RViz to work

### 07/21

- Updated the other OT-2 and succesfully ran GET method so I know that the HTTP functionalities are working
- Found a lot of issues connecting to LoCoBot with WSL2 (I think that a Linux partition would be a lot smoother)
- Fixed an issue with one of the LoCoBot's arm motors and got the arm and gripper to move.

### 07/22

- Looked into ROS2 for LoCoBot. It cannot run humble because 22.04 is not supported, so the ROS1-ROS2 bridge will probably be best.
- Work on sending a protocol for the OT-2 through HTTP

### 07/25

- Figured out how to upload, run, and delete protocols from the OT-2 through HTTP with Kyle's help

### 07/26

- Figured out how to move LoCoBot arm with Cartesian coordinates, and wrote script to move around tube in a tube rack.

### 07/27

- Learn about 3-D printing techniques for printing a new LoCoBot gripper with a wider grip to pick up plates.

### 07/28

- Continued learning about 3-D printing and worked on new gripper in Fusion 360.

### 07/29

- Continued working on a gripper and started a print.

### 08/01

- Picked up grippers and tried them on the LoCoBot. Used some foam tape as grip, but there is not a very tight grip still, so it is able to pick up plates but the grip is not tight enough to put back in the plate down accurately.

### 08/02

- Tried rubber material for the gripper to have better traction.
- Designed gripper with more surface area to grip.

### 08/03

- Wrote script for LoCoBot to follow objects.

### 08/04

- Set up Ubuntu on an external SSD so that controlling LoCoBot remotely will have less lag than VM.

### 08/05

- Go over needs of LoCobot gripper. The gripper would need to be able to reach deeper in order to pick up tip racks.
- Discuss new project on UR5e.

### 08/08

- On trip to NY

### 08/09

- Begin looking at UR5e ROS2 repository.
- Tried to connect to snowcrash, but unable to ping robot.

### 08/10

- Got properly connected to snowcrash.
- Running the UR ROS2 drivers causes a hardware unreadable error.
- Met with Kyle to learn about packaging and cleaning up driver repositories.

### 08/11

- Updated external control program on UR5e.
- Tried Galactic version of ROS2 driver, which don't show the error, but disconnects and reconnects to the robot every few seconds.

### 08/12

- Looked at Raf's ROS1 repository to see what may be going wrong with ROS2 driver.

### 08/15

- Updated PolyScope version on UR5e
- RViz now shows the correct position of the robot.

### 08/16

- Continued looking at UR repository.
- Talked with Doga about progress and problems on UR5e
- Talked with Doga and Raf about plans for Henrybot.

### 08/17

- Went over packages and code in UR repository with Doga

### 08/18

- Tried remote mode on the UR5e and the connection issue does not occur on Galactic, but Humble still shows hardware unreadable.
- Figured out how to send commands to arm when running with fake hardware and able to see movement in RViz.
- Found that the default controller specified in the UR repository is not actually the default controller (scaled joint trajectory is actually default, but joint trajectory was specified as the default one)
- Found scaled joint trajectory causes an error, but join trajectory does not activate the needed controller when running on real hardware (works in simulation)

### 08/19

- Learn about ROS controllers.
