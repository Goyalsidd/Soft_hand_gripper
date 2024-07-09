# Soft Robot Gripper for Patients with Diabetic Neuropathy
A gripper that works on air pressure and controlled manually to help the patients with diabetic neuropathy grab the objects.
It has 4 degrees of freedom:
    a) Rotational (Arm – z axis)
    b)Rotational (Car – y axis)
    c)2 Translational (Car – x&y axis) 
Process:
We started with 3D printing the mould for our soft gripper and then poured LSR into it, the gripper was made after letting it dry for 24 hours. 
We also designed a 4 way valve for the gripper which connects the air pipe to the four outlets, so that the air get uniformly distributed into all the 4 arms of the gripper.
A chassis for the car was laser cut out of a wood plastic board.
We assembled the parts of the car and uploaded the code for the servo and motors (wheels) into the ESP32 modules to complete the crane.
Finally the gripper was mounted at the end of the arms connected to the servo, gear composition.

Constraints:
Due to a time constraint the Robot is manually commanded, and could not be automated in terms of the servo motor that controls the gripper’s movements as it requires a wired input from the laptop.
Even though we managed to make the car wirelessly move through inputs from a mobile, the air pumps failed to deliver adequate pressure which forced us to use an external pressure source.

Components used:
ESP32                      
L298n
Jumper wires
Servo motor(MG996R)
DC motors 
Power Supply (Battery)
Wheels
Wood Plastic Composite(WPC) board
Gears
3D printed 4 way valve
Liquid Silicone Rubber (LSR)

The Analysis:
We tried to reduce the angular velocity of the gripper arm using the reduction provided by a simple gear train .
The speed ratio was 3:1 which is the ratio of the number of tooth in the driven gear to that of the driving gear.
Considering MG996R, we reduce speed of 50 rpm to 16.7rpm.

Difficulties Faced:
The gripper had holes in it with time and had leakages after it was sealed using a cloth from one side, we tried pivoting into making a new one but it failed as one of its arms ended up to be faulty, so we had to stick to the original gripper by plugging its leakages.
Since this was our first experience using LSR to shape the gripper through a mould, the gripper had leakages that needed plugging to make it work. An arm of the gripper got jammed with LSR while attempting the same, hence rendering it useless.
With time, the hole at the top that lets the 4 way valve enter broadened and made the fully functional gripper leak.




