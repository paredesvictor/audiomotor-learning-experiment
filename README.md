# Audiomotor learning experiment

This repository contains several Max Patch to explore an audiomotor map with sensors.

## Requirements
- **Max**: The Mubu Package from the Package Manager (don't forget to update)
- **Sensors**: 2 Inertial Measurement Units with a 3 axis accelerometer and (optionnaly) a 3 axis gyroscope

## How to
0. Clone the repository, the repo weight around 500Mo due to .wav sound files.
1. Open 'catart_read.maxpat', click 'add corpus' and select the '.mubu' file in the 'corpus' folder
2. Select 'mouse' as input, click 'init' and turn on the ezdac. You should be able to move with your mouse in the space and hear sounds
3. Sensors:
  - open the subpatchers: 'p input' --> 'p accelerometers' --> 'p sensors'
  - follow the instructions to link your sensors output to the patcher inputs
  - put sensors on your dominant arm
4. Select 'sensors' as input. Now the cursor should move according to your arm position.

## Sensors position on arm and forearm
![alt text](./readme-assets/arm.jpg) ![alt text](./readme-assets/forearm.jpg)

Only the direction of the first component (X) that you send to the outlets of the 'p sensors' subpatch matters, Y and Z can be directed wherever you want.
