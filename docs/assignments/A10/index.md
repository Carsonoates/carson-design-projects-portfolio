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
