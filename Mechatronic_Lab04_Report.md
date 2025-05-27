**Report of Lab 3: Robot**

|         Name         |
| :------------------: |
| **Truong Minh Nhat** |
|  **Dinh Thanh Ha**   |


The Robot program contains 4 main movements, with each of them having specific directives for the robot arms:

1. `MoveJ`: denotes “move joint”, this allows the movement of the robot arms in the 3 possible planes of movement, x, y, and z, with no restriction as long as the joint allows it  
   1. `origin`: denotes the original location that the robot will return to when it is done executing everything.  
   2. `pre_pick`: denotes the first position the arm moves to pick up the block; it will hover over said spot.  
2. `MoveL`: denotes “move linearly”, this allows the robot to only move in a specific axis of x, y, or z.   
   1. `pick_pos_1`: The robot moves down on the y-axis to the block, into the position to be ready to grab the block.  
   2. `Wrist Connection`: Command the robot’s claw to grab onto the block.  
   3. `pre_pick`: return the robot arm to the first position from the first MoveJ, 1.b.  
3. `MoveJ`: means “Move Joint”, its meaning has been explained as above   
   1. `pre_place`: Position before the robot drop the block into the destination slot   
4. `MoveL`: Move Linear, meaning is as above   
   1. `place_pos_1`: The arm move down the y-axis (vertically) to put the block into designated slot   
   2. `Wrist Connection`: disengage the claw that currently grabbing the block   
   3. `pre_place`: Position before the robot drop the block into the destination slot (the same position in step 3)

