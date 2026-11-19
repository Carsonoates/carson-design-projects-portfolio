# A11 – Motor Selection Loose Screws
For this assignment, our group (Carson, Maddux, Chris) was tasked with selecting a motor to attach to the frame designed in A10, using the same constraints. We accomplished this by using Torque/Speed charts and the aforementioned calculations to find the right motor to power our tensile tester. 

<img width="596" height="208" alt="assignment_heading_reference" src="https://github.com/user-attachments/assets/8aa1941f-754a-4d78-8c98-aa07da0ebe4b" />

## 1. Motor Selection

(Chris Chorny)

I started by using the 4 mm lead of the screws to find the motor speed range needed for the crosshead. I then used the required torque per motor and the factor of safety to decide which motor would work. We selected the McMaster 6627T924 NEMA 34 stepper motor and checked its torque-speed chart at our operating speeds. The motor drawing and the correct chart for this specific motor are below.

<img width="507" height="391" alt="motor_dimensions" src="https://github.com/user-attachments/assets/03336e0b-4cee-40b5-bca9-6987f5dffdcf" />

<img width="519" height="393" alt="motor_torque_speed_correct" src="https://github.com/user-attachments/assets/59b7c333-990c-41ff-9376-79ac574065c4" />

<img width="1112" height="1489" alt="handwritten_page_1" src="https://github.com/user-attachments/assets/e0c7ff23-601f-43aa-abf1-f7fb97e973af" />

## 2. Motor Mounting Plate

(Chris Chorny)

I designed the motor mounting plate in SolidWorks using 6061-T6 aluminum. The plate is 4 by 4 inches, with a selected thickness of 0.25 inch. The mounting holes and center opening were laid out around the NEMA 34 motor dimensions, as shown in the hand-drawn plate layout. My initial minimum-thickness calculation was incorrect, so instead of relying on that result we went with the more substantial quarter-inch plate. I later worked through a simplified bolt-hole bearing-stress check, shown in my handwritten work. That check does not by itself verify plate bending or the full mounting assembly.

<img width="2924" height="3958" alt="handwritten_page_3" src="https://github.com/user-attachments/assets/3d002fce-3e85-4fbf-9fa6-dc818e8c7246" />

<img width="2267" height="2939" alt="handwritten_page_2" src="https://github.com/user-attachments/assets/7af900b1-0064-4431-9536-7893754ca86d" />

## 3. Coupler Selection and Analysis

(Chris Chorny)

For the connection between the motor and lead screw, I selected the McMaster 61005K133 rigid keyed coupler. I treated the coupler as a hollow circular shaft for a basic torsional shear check. The handwritten work shows how I estimated the minimum wall thickness and compared it with the much thicker selected part. The calculation uses an assumed steel strength and does not check the keyway, clamping screws, or whether the actual shaft ends match both coupler bores.

<img width="391" height="527" alt="coupler_product_dimensions" src="https://github.com/user-attachments/assets/c4532faf-7686-439c-a8fd-5b478f8f8428" />

<img width="2267" height="2939" alt="handwritten_page_2" src="https://github.com/user-attachments/assets/4c59e095-54f4-47a8-adef-51dbdf92193a" />

## 4. Frame Connection Brackets

(Chris Chorny)

We selected two McMaster 5537T665 gusseted corner brackets to attach the top frame to the vertical supports. The brackets are spaced about 300 mm apart. I used the motor torque to estimate a force at the frame connections, then used a simplified bending model to make an initial stress comparison. The effective bracket thickness and material yield strength used in the handwritten check were assumptions, so this is only a preliminary check and not a complete verification of the triangular gusset or the T-slot fasteners.

<img width="2924" height="3958" alt="handwritten_page_3" src="https://github.com/user-attachments/assets/26d72f16-1036-4784-9ac9-6f3d0ce36934" />

### FEA

(Maddux)

For the FEA, we decided to test the bottom part of our frame. We used a normal mesh and had 1000N force pushing up and a 4.12Nm torque acting on the holes of the frame.

<img width="472" height="371" alt="image" src="https://github.com/user-attachments/assets/87ac26f3-34db-4816-9e73-8c37c6c50a1e" />

<img width="469" height="404" alt="image" src="https://github.com/user-attachments/assets/10915d10-569b-4115-93a7-1c05f32dbce2" />

<img width="470" height="215" alt="image" src="https://github.com/user-attachments/assets/b7e77f4b-392c-4059-a794-ebee3e5aa3bf" />

<img width="467" height="208" alt="image" src="https://github.com/user-attachments/assets/703215ca-40f1-4c7a-ae6e-87b3fe31efbc" />

After running the FEA test, the stresses never exceeded our max yield strength and diffraction was in the allowable range as well. Since these values were acceptable, we decided not to improve the design of the frame.

This section covers the floating bearing support required for the continued two-lead-screw tensile tester design. The scope is to select a standard bearing, design a housing that attaches to the Grainger T-slot frame, and consider the fit and movement needed for a floating support.

## 1. Bearing Selection

(Carson Oates)

I selected McMaster 2349K416, a sealed 6004-size radial ball bearing. It has a 20 mm nominal inside diameter, a 42 mm outside diameter, and a 12 mm width. I used these dimensions to size the bearing pocket in the housing model.

<img width="385" height="583" alt="bearing_product_dimensions" src="https://github.com/user-attachments/assets/b06edc17-99ad-4a0b-b688-5d5d8881d8ec" />

## 2. Floating Bearing Housing

(Carson Oates)

I modeled a rectangular support in SolidWorks with a recessed bearing pocket and four mounting holes. The design is intended to attach to the Grainger 40 by 80 mm T-slot framing. The housing and bearing are shown separately so the pocket and mounting layout are easy to see.

<img width="792" height="547" alt="floating_bearing_housing" src="https://github.com/user-attachments/assets/a325190d-a0a8-4cb7-a70d-13484b7014b4" />

<img width="559" height="683" alt="motor_mount_solidworks" src="https://github.com/user-attachments/assets/b830df99-6831-4800-9fb2-04821bb1a4d3" />

## 3. Fits and Tolerances

(Carson Oates)

I used the supplied Class RC3 table as a reference when considering clearance and how the floating support should work. RC3 describes a running clearance between mating hole and shaft surfaces. It does not automatically specify the correct bearing outer-ring-to-housing fit. That housing fit and the amount of axial movement would need to be checked against the actual bearing and assembly before manufacturing.

<img width="232" height="353" alt="rc3_fit_table" src="https://github.com/user-attachments/assets/7e2a7066-75fa-40dd-ae3f-e2b858ec3a6f" />

## 4. Assembly Considerations

(Carson Oates)

The housing is meant to support the lead screw while allowing the intended floating movement. One limitation is that our lead screw is fully threaded M20: a nominal 20 mm bearing bore doesn't provide a proper running journal on those threads. The current model shows the intended layout, but a suitable bearing journal or other engineered interface would be needed for a real build.

## Material and Labor Costs

| Item Number | Quantity | Name | Cost/Item | Cost | Link |
| --- | --- | --- | --- | --- | --- |
| 1 | 2 | Lead Screw 7549K78 | $34.52 | $69.04 | [Link](https://www.mcmaster.com/7549K78/) |
| 2 | 2 | Precision Flange Nut 7549K22 | $82.27 | $164.54 | [Link](https://www.mcmaster.com/7549K22/) |
| 3 | 1 | Flange Screws 91251A542 | $12.95 (50 Pack) | $12.95 | [Link](https://www.mcmaster.com/91251A542/) |
| 4 | 1 | Framing System 804T48 | $245.87 | $245.87 | [Link](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48) |
| 5 | 2 | Framing Brackets 5537T665 | $15.26 | $30.52 | [Link](https://www.mcmaster.com/5537T665) |
| 6 | 2 | Coupler 61005K133 | $69.83 | $139.66 | [Link](https://www.mcmaster.com/61005K133) |
| 7 | 2 | Stepper Motor 6627T924 | $692.16 | $1384.32 | [Link](https://www.mcmaster.com/6627T924) |
| 8 | 1 | Motor Mount Bolts 91280A326 | $20.50 (100 pack) | $20.50 | [Link](https://www.mcmaster.com/91280A326) |
| 9 | 8 | Floating Bracket Bolts 92562A271 | $3.67 | $29.36 | [Link](https://www.mcmaster.com/92562A271) |
| 10 | 1 | Bracket-To-Frame Bolts 94036A825 | $7.33 (10 pack) | $7.33 | [Link](https://www.mcmaster.com/94036A825) |
| 11 | 2 | Bearing 2349K416 | $23.35 | $46.70 | [Link](https://www.mcmaster.com/2349K416) |

| Person | Work Time | Payment |
| --- | --- | --- |
| Carson | 4 hours | $140 |
| Maddux | 5 hours | $175 | 
| Chris | 6 hours | $210 |
| Total Price: $ | $2,675.79 |

## Final Design (Carson)
Here was the final design of the Tensile Tester

<img width="597" height="611" alt="Screenshot 2026-11-18 222736" src="https://github.com/user-attachments/assets/82bc940a-9511-432b-a112-49b6279ba30e" />

## Drawings (2157-Maddux)

Below are the drawings of each part that we designed on our own to complete this tensile tester. Each drawing has 4 different views with sufficient dimensions and the correct title card. 

<img width="466" height="330" alt="image" src="https://github.com/user-attachments/assets/e6d844ea-f528-4c44-b68f-eb4a5f84da08" />

<img width="468" height="335" alt="image" src="https://github.com/user-attachments/assets/f1ec409b-24fa-4093-8d8e-7aed651ce625" />

## Lessons Learned
This assignment taught us a lot about how the full design process works and how to work as a team. We gained first-hand experience designing from scratch, and it was a cool experience. One thing that really caught us off guard was the total cost. Aside from that, we learned a lot from the project's optimization and assembly aspects.

This assignment took a total of 15 hours combined.

Downloads here: [CAD](Loose_Screws_A11_FrameCAD.zip) [Drawings](Loose_Screws_A11_Drawings.zip)





