# A4 – Motor Mount

## Objective
For this assignment, I was tasked with creating a motor mount using the motor found [here](https://www.omc-stepperonline.com/brushed-24v-dc-gear-motor-3-6kg-cm-46rpm-w-99-5-1-planetary-gearbox-pa28-28245800-g100) as a reference. The goal was to use the motor's dimensions to design a mount that could withstand a 300 N force with a max deflection of 0.3 mm. To simplify the assignment, we were told to ignore the weight of the motor and to take into account a safety factor of 3, which would cover the holes for the motor shaft and bolts.

<img width="768" height="295" alt="image" src="https://github.com/user-attachments/assets/41089000-7f11-4026-a2b5-7fa2b3a63847" />

## Designing Feature 1

Before starting the project, I spent 15-20 minutes brainstorming how I wanted to tackle this assignment. I first looked at the description and dimensions of the motor to understand its size and listed the values I thought mattered most. I then began sketching a few ways I wanted the mount to look before settling on a final design. I then listed out a few footnotes before beginning the rest of the assignment.

<img width="803" height="336" alt="image" src="https://github.com/user-attachments/assets/0e0ff738-f6cd-4520-abf2-257f95e2acde" />

### a. 
The first feature is designed with the idea that it will hold the motor in mind. As such, a hole will be placed in the center of the feature's cross-section. With the game plan laid out, I began listing the knowns and unknowns for the first feature.

<img width="267" height="228" alt="image" src="https://github.com/user-attachments/assets/1192411f-2511-42da-98fb-a9e5e94ad557" />

### b.
The next step was to create a free-body diagram, which I used to solve for some of my unknowns. I also calculated the maximum allowable stress for later use.

<img width="452" height="204" alt="image" src="https://github.com/user-attachments/assets/2be90014-a3b2-49db-bca9-91f613e30eaf" />

### c/d.
I then began to calculate the cross-section of the feature using the equation for stress given here: Mc / I. Since I had already predetermined a base and length measurement, I substituted some variables out in favor of equations to find the height of the feature. Once the height for stress was found, I then used a similar process using deformation instead. Using the equation for deformation and the previous substitutions, I found the height for deformation. When comparing the two values, I found that the height for deformation was larger than the height for stress, meaning the height for deformation would be the best option. I rounded the value up to a flat value of 20 mm to make calculations and spacing for the CAD model easier, and compared the max allowed stress and deformation to calculated values to check if the dimensions would suffice.

<img width="805" height="162" alt="image" src="https://github.com/user-attachments/assets/5baef319-ff42-4c63-820f-72698a628b0d" />

<img width="762" height="220" alt="image" src="https://github.com/user-attachments/assets/30dd24eb-3ea4-498f-8ee2-3ddfcfeee1ef" />

## Designing Feature 2

Now we move on to feature 2. This feature will be attached to the wall, so holes will be placed at a uniform distance as clearance for the bolts. To solve for the cross-section of feature 2, we will use the same process as we did for feature 1. This means using the stress and deformation equations to solve for the missing dimension, and comparing those values to determine which is greater. Because I want both features to be as similar as possible, I used the same variables as last time to solve for the height. This makes the calculations easier, as they are the same as feature 1.

### a/b.
First, we list our knowns and unknowns, draw our free-body diagram, and use that to find some of the unknowns.

<img width="794" height="242" alt="image" src="https://github.com/user-attachments/assets/e3b66c26-9606-4a82-aadf-fc2192bc8447" />

### c/d. 
Then we find our equations and solve them for our respective height values, and compare them to see which is the best fit. Finally, we plug the values back into the equations to see if they satisfy our requirements.

<img width="786" height="170" alt="image" src="https://github.com/user-attachments/assets/54f1e8ec-5932-4930-a526-8cad6cf1d2b4" />
<img width="795" height="238" alt="image" src="https://github.com/user-attachments/assets/5d7da1d4-e636-421f-bd29-48d9c70863cf" />

## Isometric Sketch
Before moving on to the CAD model, I quickly hand-sketched the motor mount and labeled the dimensions found on the sketch for a general idea of what I wanted the model to look like.

<img width="310" height="286" alt="image" src="https://github.com/user-attachments/assets/dd44f73a-bc95-4e7e-9cb5-75921267ebe4" />

## The CAD Model

The last step was to model our mount in CAD software using the dimensions we found through calculations and from the motor's descriptions. I decided to split the motor mount into two parts and assemble them later on. For feature 1, I used the exact dimensions I listed out before adding the hole for the motor. For the hole, I created two cuts, one for the gearbox and one for the shaft. The gearbox hole is 16 mm deep with a diameter of 28.25 mm for a clean fit, and the shaft hole pierces the entire part with a diameter of 6.5 mm.

<img width="807" height="621" alt="Screenshot 2026-09-17 004125" src="https://github.com/user-attachments/assets/b17592b4-a04f-467e-8fd4-2ab633014e36" />
<img width="1019" height="533" alt="Screenshot 2026-09-17 004407" src="https://github.com/user-attachments/assets/959b2b49-5519-4e1c-8ab8-35d0865f40eb" />
<img width="669" height="817" alt="Screenshot 2026-09-16 221904" src="https://github.com/user-attachments/assets/aa2fefa0-2abb-47bd-bdae-07b8fd89f587" />

Feature 1 and feature 2 have the same dimensions, so the only difference between the two parts is the hole placed in them. Since feature 2 will be attached to the wall, holes with a 3.4 mm diameter were added uniformly, with enough space for feature 1 to attach to the bottom of it.

<img width="726" height="775" alt="image" src="https://github.com/user-attachments/assets/a332555a-b23b-46dc-b3b4-0833fd74e778" />
<img width="811" height="774" alt="Screenshot 2026-09-16 221853" src="https://github.com/user-attachments/assets/312702f1-3f89-40af-894a-4cc12be5a478" />

Once the parts were made, I assembled them to create the final product.

<img width="806" height="767" alt="Screenshot 2026-09-16 221823" src="https://github.com/user-attachments/assets/9782d281-5a7c-48d3-8093-3efc3e788f71" />

## 2157 Extra

Because I am in MEGR 2157, I was given an additional task of creating a drawing of the motor mount using CAD software. To accomplish this, I used SolidWorks' drawing feature and began setting up the sheet in a third-angle projection, as I was instructed. With the help of some SolidWorks tutorials and trial and error, I created the drawing in the projection, added dimensions, and filled out the title block.

<img width="1097" height="841" alt="image" src="https://github.com/user-attachments/assets/8ee7a5bc-ffe8-4ba0-876d-ab9f99afe501" />

## What I learned from this assignment

I found this assignment to be really interesting. While I do believe I created a pretty dysfunctional motor mount, I still learned some skills related to the process of design. The biggest thing I learned from this was how to use an external object, like the motor, to help create parameters for the design process to follow. On the CAD side, this was the first time I had experimented with the drawing feature and learned about the different ways to place the drawings.

This assignment took me 5 hours to complete.

SolidWorks Downloads:
[Feature 1](./Figure_1_CMO.SLDPRT) [Feature 2](./Figure_2_CMO.SLDPRT) [Motor Mount Assembly](./Motor_Mount_CMO.SLDASM)
