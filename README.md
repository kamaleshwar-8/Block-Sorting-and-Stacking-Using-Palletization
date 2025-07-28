# Overview

This project focused on implementing a block sorting and stacking system using the Epson VT6-901S 6-axis robot. The objective was to pick blocks arranged in a 1×9 grid layout (acting as a pallet), measure their individual heights, and stack them at a single drop point—one on top of the other—based on height values. This was then followed by reversing the process, where the blocks were returned to their original positions in the grid.

# Key Features and Workflow:

- Pallet Picking: We utilized the Pallet command in Epson RC+ to define and iterate through the 9x1 grid positions for systematic picking of blocks. This simplified positional control and allowed us to use looping logic for efficient handling.
  
- Height Measurement and Accumulation: As each block was placed on top of the previous one, we calculated the cumulative height using a for loop, adding the height of each block to determine the Z-coordinate for placement.
  
- Reverse Sorting: After stacking, the process was reversed using the same logic—reading the stacked order and returning the blocks to their corresponding original pallet positions based on their order.
  
- Pneumatic Gripper Integration: This was our first exposure to using a pneumatic gripper, which operated using air pressure to suck and release the object. The gripper was programmed to synchronize its operation with the robot’s motion sequence.


# Result

Video link : https://youtu.be/l6jhKtryECY

<img width="1531" height="855" alt="image" src="https://github.com/user-attachments/assets/9dabb64a-3f85-4acb-bd69-96b4a62609ac" />

<img width="1460" height="792" alt="image" src="https://github.com/user-attachments/assets/cc193e19-ca26-4ebd-871e-18ea88d224f6" />

<img width="1477" height="788" alt="image" src="https://github.com/user-attachments/assets/19f3f77b-55a6-494f-8399-88cb0e4d46c2" />
