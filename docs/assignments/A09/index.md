# A9 – Pulley System Design

## Objective
- Use numerical analysis to design a pulley system

## Assignment Details
For this assignment, I was tasked with designing a pulley system using pulleys with a diameter of 3 inches, a rotational speed of 1500 RPM, and a static belt tension of 5 lbf. To start the assignment, I began with the belt

## Belt Analysis (Part 1)
Finding the proper belt for the pulley required a few calculations to find the forces while the belt is pulled taut and while the belt is hanging loose. These can then be used to find the belt diameter and outer circumference. The first thing I did was list out the knowns and unknowns I currently had.

<img width="543" height="350" alt="image" src="https://github.com/user-attachments/assets/0cbe30f7-f35f-4e97-8372-bb54740e7784" />

With an idea in mind for what we need to find, I began writing out the equations and algebraically solving for the variables we're missing.

<img width="792" height="272" alt="image" src="https://github.com/user-attachments/assets/9c18ec11-dca2-4981-b7dc-5bbbfd72d940" />

Looking at the FBD and the parameters for the assignment, we can see that theta is equal to pi since both circles are 180 degrees from each other, and our coefficient of friction mu is 1 since no slippage will occur. Plugging these values into the equations, we can find the values that our belt needs to match to properly function.

<img width="571" height="278" alt="image" src="https://github.com/user-attachments/assets/f51431d8-7df0-4d81-9b67-b8daf9c116f4" />

The best fit for our pulley that I could find on McMaster is this [belt](https://www.mcmaster.com/3044K608/) I found here. The diameter is large enough, and the outer circumference fits what we are looking for. A 5/16 diameter belt would have fit better; however, there was no belt available with the proper circumference.

## Shaft Analysis (Part 2)
Up next was to design the shaft for the pulley system. We needed to find the diameter for a shaft made of 1060 hardened steel that can support the 5 lbf torque being applied to the system. This process started with listing what we know and what we need to know to find our area. I also used [Matweb](https://www.matweb.com/search/datasheet.aspx?matguid=ecd1f5f21fe943e7a892d70ea57a43e8&ckck=1) to find the yield strength for our material, which is listed as 485 MPa or 70300 psi.

<img width="478" height="188" alt="image" src="https://github.com/user-attachments/assets/a8a17b70-04bb-4983-8a9c-f660513d2a62" />

I then began to solve for the diameter of the shaft using algebraic methods.

<img width="300" height="78" alt="image" src="https://github.com/user-attachments/assets/96ca5ba0-1c51-42a3-9f78-644d74dba580" />
<img width="387" height="86" alt="image" src="https://github.com/user-attachments/assets/8a10e2e2-7f66-4207-8c1f-f2d13875fb0b" />

Which I then used to find the geometry.

<img width="646" height="49" alt="image" src="https://github.com/user-attachments/assets/20211875-bb48-4857-8313-58c8e96e08ab" />

## Bearing Analysis (Part 3)
Now that we know the shaft's diameter, we can find the bearings that will be attached to it, starting with the knowns and unknowns.

<img width="436" height="172" alt="image" src="https://github.com/user-attachments/assets/221f00ec-d59a-4e1c-ad75-c8fe33703a9a" />

To find the material needed for the bearings, we need to find out the pressure and velocity that our pulley system outputs. This will give me the PV limit that narrows down the list of materials I can use. First, I used algebra to find the equations that define the geometry.

<img width="421" height="129" alt="image" src="https://github.com/user-attachments/assets/3a4536ae-1149-4215-a566-be71f20b7900" />

Then I used the shaft diameter and the force I found earlier to find the pressure, and I converted the revolutions per minute to feet per minute to find the velocity. Multiplying these numbers gives the PV limit a material must withstand to fit our pulley.

<img width="416" height="38" alt="image" src="https://github.com/user-attachments/assets/1fb9ec2e-0476-49db-9739-3c0225ca89f2" />
<img width="983" height="679" alt="image" src="https://github.com/user-attachments/assets/07a420be-29b6-4013-87b1-5089d5dc00a8" />

Using Table 4 found on page 2440 of the handbook, I can see that the only option available is lubricated Graphite with a PV limit of 150000.

## Frame Analysis (Part 4)
The last step for this assignment is to design a frame to support the pulley system. I treated the frame as a simple axially loaded bar with forces at both ends, with F equal to 2*T.

<img width="385" height="111" alt="image" src="https://github.com/user-attachments/assets/3f55c3f9-38c4-4881-a6a4-b533dc8cde34" />

Using this kind of geometry, we must prioritize stress over density when picking a material. Using an Ashby Plot I found, I began looking for a suitable material.

<img width="959" height="731" alt="image" src="https://github.com/user-attachments/assets/01420aa9-ca94-4dc9-8308-ed2f8bc3c4a7" />

The proper material depends mostly on what constraints I have regarding the frame's specs, specifically the weight and area of the frame. If the area were very limited, a stronger material like some aluminum alloys would provide a good amount of support but would add more weight as a trade-off. Woods, aluminum alloys, and steels would all serve as good choices for a frame, but more information about the room and weight requirements would be needed to round out the exact best material. For this assignment, I think an aluminum alloy would suffice for a frame.

## What I've Learned
This assignment has shown me how important each material is for its respective part of the system. For the bearings, there was no other option other than the lubricated graphite available for me to use with my calculated values. Assuming the belt was made of polyurethane rubber already affected the calculations for the entire assignment.

This assignment took me 3 hours.






