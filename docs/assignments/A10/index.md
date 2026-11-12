# A10 – Lead Screw Design

## Objective
- Develop a lead-screw-driven crosshead.
- Ensure accurate, repeatable load application to 2kN with minimal crosshead deflection and misalignment.
- Provide robust specimen gripping, simple calibration provisions (mechanical), and safe ergonomic operation.

## Leadscrew Diameter (1 Carson)
To start the assignment, we need to determine the minimum lead screw diameter based on a few constraints. It needs to withstand a load capacity of 2 kN, have a speed range of 1-50mm/min, a minimum length of 18 inches, and a safety factor of 4. Starting with the knowns and unknowns, I solved the equation algebraically and plugged in the known values to find a minimum diameter of 4.51 mm. This led me to find a good fit for a screw on Roton [here](https://www.roton.com/product/trapezoidal-steel-screw-right-60866/).

<img width="496" height="242" alt="CO picture 1" src="https://github.com/user-attachments/assets/686e9c30-cbfe-41f0-9d23-8944986779ab" />

## Rotational Speed (2 Carson)
Next, I found the rotational speed range. Using what we know about linear speed and our knowns, I found the equation and values for the rotational speed range at minimum and maximum speeds of 0.25 and 12.5 RPM, respectively.

<img width="518" height="121" alt="CO picture 2" src="https://github.com/user-attachments/assets/4138b3d7-7928-4d3f-a4b8-3d0cc7116fa7" />

## Torque (3 Carson)
The last thing we needed for the screw was the maximum torque required to provide 2 kN of tension. For this section, I used the equation we found in class to calculate the torque required to resist the screw's movement under load. After researching the coefficient of friction between steel and bronze and learning about trapezoidal screws, I found the torque to be 3.5 Nm between the two screws.

<img width="579" height="302" alt="CO picture 3" src="https://github.com/user-attachments/assets/7bcef1b8-8221-4efd-b12a-6681b63c275d" />

However, when I went to download the CAD model for the screw, I found that Roton does not provide models, so I needed to find a replacement. Thankfully, McMaster had a very similar [screw](https://www.mcmaster.com/7549K78/), which only required a torque recalculation, yielding a torque value of 4.12 Nm.

<img width="332" height="108" alt="CO picture 4" src="https://github.com/user-attachments/assets/05a48512-097f-44c8-9d9c-5015e77b5ad1" />

## Nut/Flange Calculation (4 Carson)
Along with the screw, we need a compatible flange. Using an equation I found for bending stress in the lecture and finding a compatible [flange](https://www.mcmaster.com/7549K22/) on McMaster, I was able to find a compatible flange that satisfies the constraints given.

<img width="515" height="288" alt="CO picture 5" src="https://github.com/user-attachments/assets/7ce3e201-7671-49a5-a3dc-1d5f6ccec5ee" />

## Crosshead (1 Maddux)
For the cross head of this tensile tester, there was a lot of creative freedom to design so many of the dimensions are based on my judgment calls but I did try and find as many concrete values as possible.
To start out on this cross head I decided to draw out what it would look like once it was all assembled and dimension it like that. The values of the lead screw, flange nut, screws for the flange nut, and forces acting on the crosshead came from previous parts of this project, and the rest of the values were made by me. 

<img width="780" height="340" alt="image" src="https://github.com/user-attachments/assets/21ff42d2-7b90-4a0e-910c-2c644b561439" />

I decided to make this crosshead out of aluminum 6061-T6 since it is very strong relative to its weight. The only thing that needed to be calculated for this crosshead was the minimum height requirement.

<img width="783" height="730" alt="image" src="https://github.com/user-attachments/assets/b8e2e4d4-e15e-4523-a140-f8b3b8b13a9e" />
<img width="781" height="243" alt="image" src="https://github.com/user-attachments/assets/f24ab0fe-1a0a-4e9e-905a-1d66190e950d" />

I found that the minimum height requirement was 12.79mm but I decided to make the height 40 mm to ensure that everything works well and to ensure that the screws for the flange nut have enough depth.

With my design I did add a thread to the crosshead section that would connect the cross head to the load cell. The thread that I used was .2500-28UNF since the maximum forces applied didn’t exceed 300lbf. 

I then created my three multiview drawings making sure to dimension out everything.

<img width="782" height="429" alt="image" src="https://github.com/user-attachments/assets/4c18ede5-3c0b-4788-9db6-7d32bfcf10e3" />

## CAD (2 Maddux)
Here are my global variables.

<img width="784" height="200" alt="image" src="https://github.com/user-attachments/assets/18968c18-c231-4df2-b0ab-944c44e6b944" />

Here is my drawing of crosshead and it being extruded.

<img width="785" height="403" alt="image" src="https://github.com/user-attachments/assets/c8d39d12-e524-4df7-b12e-7bf69fd4e60c" />

Here are my drawings of the circles that are extruded and cut from the crosshead.

<img width="781" height="719" alt="image" src="https://github.com/user-attachments/assets/9e893c7e-36bc-4ceb-8d02-12c8e80869fe" />

Here is the thread that connects the crosshead to the load cell.

<img width="785" height="417" alt="image" src="https://github.com/user-attachments/assets/035baea1-7652-47a7-a853-2e295c046e76" />

Here is the part that I am using for the frame. This is a T-slot framing system from the Grainger website, [item #804T48](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48), just modified by removing 2628mm from its length and adding holes for the lead screws to go through.

<img width="783" height="293" alt="image" src="https://github.com/user-attachments/assets/74f3873b-dfe0-435d-bbe6-c5e6515739e3" />

## Assembly of Tensile Tester (3 Maddux) 
The assembly of this tensile tester consists of 17 different parts, requiring 37 mates to make it functional, all consisting of coincident and concentric mates. The only problem was I couldn't figure out how to have the crosshead to move independently so to move the lead screws up and down you have to lift the whole frame with it.

<img width="780" height="769" alt="image" src="https://github.com/user-attachments/assets/ad6d7634-793c-4bc1-a5a1-3dfcd13e8e85" />






| Item Number | Quantity | Name | Cost/Item | Cost | Link |
| --- | --- | --- | --- | --- | --- |
| 1 | 2 | Lead Screw 7549K78 | $34.52 | $69.04 | [Link](https://www.mcmaster.com/7549K78/) |
| 2 | 2 | Precision Flange Nut 7549K22 | $82.27 | $164.54 | [Link](https://www.mcmaster.com/7549K22/) |
| 3 | 1 | Flange Screws 91251A542 | $12.95 (50 Pack) | $12.95 | [Link](https://www.mcmaster.com/91251A542/) |
| 4 | 1 | Framing System 804T48 | $245.87 | $245.87 | [Link](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48) |
| Total Price: $410.13 | 
