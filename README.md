# What this does
- simulates a command swerve drive like a video game
- will simulate an additional subsystem soon
- hopefully simulates vision soon

# How it does it
- java
- generated project through pheonix tuner and maplesim
- uses advantagescope's 3d field and built in kitbot assets to simulate robot drive

# How use simulation
1. prep advantagescope
- help -> show assets folder
- either:
    - create a folder for your robot's 3d model according to the advantagescope docs
    - go into the parent directory, then copy the directory autoAssets/Robot_2024KitbotV2 to the userAssets folder
2. run this code
- download it and unzip it if neccessary
- open in in FRC's VScode
- ctrl+shift+p
- type and enter "WPILIB: Simulate robot code"
- select simulation GUI
3. configure simulation
- open the new robot simulation window
- select teleoperated from the list of robot modes in the upper left
- drag your method of choice to control the robot to joystick 0 (usually a USB-connected xbox controller or keyboard 0 if you don't have a controller)
- if on keyboard 0, right click it in the system joysticks menu and select edit keyboard 0
- for Axis 0, set increase to w and decrease to s
- for Axis 1, set increase to d and decrease to a
- you can set them to whatever you want technically, but this is standard WASD controls
4. configure advantagescope
- go to advantage scope
- click the plus in the upper right corner, then select 3D field if 3D field is not already in the top bar
- click on where it says 3D field on the tob bar
- in the sidebar, click where it says pose to open the dropdown menu
- click and drag robotPose to the poses section under the field
- right click the direction arrow next to RobotPose, select Models, then select Crabbot if it's not already selected
5. run the sim
- use your xbox controller, WASD controls if you're using keyboard 0, or whatever other controller you've selected to move the robot while the robot simulation window is your selected window
- If movement correlation is unclear, hit the plus sign and select swerve. This screen will show you which direction (robot oriented) the bot is moving in. This codebase is by default bot oriented (working on that).

# Things I've picked up:
- git has a limit to file and repo size
- for some reason, it factors branch history into that
- gitignore is a good way to leave out compiled folders because they're practically useless to anyone besides you and the clog up your repo

# What I'm working on:
1. vision
2. arm subsystem
