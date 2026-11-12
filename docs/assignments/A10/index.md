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

# Finite element analysis (2157 students)
**Chris Chorny**

## Purpose
I compared the original and optimized crosshead in SOLIDWORKS Simulation to see how removing material affected mass, stress, and displacement. The original design is documented first, followed by the changes I made, the optimized FEA, and the final comparison.

## Original crosshead and initial setup

I started with the original crosshead design and prepared the two mounting locations for the static simulation. I made 2.57-inch-diameter circular regions and used Split Line so the mounting faces could be selected separately. I fixed these two regions and applied the downward load to the center section.

<img width="1706" height="769" alt="documentation1" src="https://github.com/user-attachments/assets/8127ad38-5204-4e29-990b-000be1f14739" />
*Figure 1. Dimensioning the 2.57-inch mounting regions on the original crosshead.*

<img width="1623" height="591" alt="documentation2" src="https://github.com/user-attachments/assets/76d0b3e9-51aa-4ff1-8931-098309ea6b8d" />
*Figure 2. Split Line faces created at the mounting locations.*

<img width="1582" height="559" alt="documentation3" src="https://github.com/user-attachments/assets/f15aa2d3-b9c5-4547-bec8-c75e67adf3a6" />
*Figure 3. Fixed geometry applied to both circular mounting regions.*

<img width="1159" height="387" alt="documentation4" src="https://github.com/user-attachments/assets/c1921d22-16b1-4b07-94b2-454cbb4dadbf" />
*Figure 4. Downward force applied at the center of the crosshead.*

## Original design: FEA results

I ran the original crosshead through coarse, medium, and fine mesh analyses. These plots provide the baseline before any material was removed. The deformation displayed in the plots is exaggerated for visibility; the actual displacement values come from the legends.

<img width="1391" height="571" alt="Original_Coarse_Displacement" src="https://github.com/user-attachments/assets/7f08c773-6e3a-49eb-847b-ad9b4f79c0a7" />
*Figure 5. Original crosshead — coarse-mesh displacement.*

<img width="1429" height="649" alt="Original_Coarse_Stress" src="https://github.com/user-attachments/assets/e15b8e5c-87a4-41ac-a0f9-0665023465a7" />
*Figure 6. Original crosshead — coarse-mesh von Mises stress.*

<img width="1371" height="646" alt="Original_Medium_Displacement" src="https://github.com/user-attachments/assets/912a12bf-e24b-4e68-97be-3d164f385cdc" />
*Figure 7. Original crosshead — medium-mesh displacement.*

<img width="1386" height="681" alt="Original_Medium_Stress" src="https://github.com/user-attachments/assets/36360768-638f-474f-b88a-619c74691174" />
*Figure 8. Original crosshead — medium-mesh von Mises stress.*

<img width="1448" height="665" alt="Original_Fine_Displacement" src="https://github.com/user-attachments/assets/78cdafa4-dd5b-4bb7-82fa-11204dda113f" />
*Figure 9. Original crosshead — fine-mesh displacement.*

<img width="1421" height="631" alt="Original_Fine_Stress" src="https://github.com/user-attachments/assets/540ed6d5-992c-4c40-bf67-96d0446e0817" />
*Figure 10. Original crosshead — fine-mesh von Mises stress.*

## Original design: mesh convergence check

I checked the original crosshead with coarse, medium, and fine solid meshes. The maximum von Mises stress and resultant displacement (URES) from each plot are listed below. The displacement values are **resultant**, not the vertical displacement component at the grip line.

| Mesh | Maximum von Mises stress (MPa) | Maximum resultant displacement (mm) |
|---|---:|---:|
| Coarse | 3.520 | 0.002155 |
| Medium | 5.414 | 0.002198 |
| Fine | 4.983 | 0.002185 |

Medium-to-fine stress change = |4.983 − 5.414| / 5.414 × 100 = **7.96%**. Medium-to-fine displacement change = |0.002185 − 0.002198| / 0.002198 × 100 = **0.59%**. The displacement is relatively stable, but the maximum stress is still mesh-sensitive. The fine-mesh result is used for the design comparison, not treated as proof of full stress convergence.

## Original design: baseline measurements

Before changing the geometry, I recorded the original mass and the fine-mesh FEA results. These values are the baseline for checking how much material I could remove and what effect that removal would have on stress and displacement.

| Measurement | Original design |
|---|---|
| Mass | 6.12 lb |
| Volume | 62.74 in³ |
| Fine-mesh maximum von Mises stress | 4.983 MPa |
| Fine-mesh maximum displacement | 0.002185 mm |
| Material yield strength | 275 MPa |

The original mass was 6.12 lb. This was the starting point for the weight-reduction work.

## Design optimization and model changes

After reviewing the original design, I sketched two rectangular pockets to remove material from areas away from the mounting faces. I added rounded transitions and fillets around the pocket edges and corners. The goal was to reduce weight while keeping the same main mounting and loading arrangement.

<img width="1409" height="741" alt="documentation5(1)" src="https://github.com/user-attachments/assets/19a5ed34-7e3e-44cc-b8e1-862380526039" />
*Figure 11. Dimensioned sketch for the two material-removal pockets.*

<img width="770" height="663" alt="documentation6(1)" src="https://github.com/user-attachments/assets/20bbf4fe-343f-40c7-835f-e76ddeb6790e" />
*Figure 12. Optimized geometry showing rounded transitions on the underside.*

<img width="983" height="706" alt="final_optimized" src="https://github.com/user-attachments/assets/eb33d095-acfd-48a1-ae36-9bd3fe5cc632" />
*Figure 13. Final optimized crosshead with two pockets and fillets.*

## Optimized design: FEA results

I then ran the optimized model using coarse, medium, and fine meshes. I compared the displacement and von Mises stress plots with the original design to see the effect of the removed material. The optimized part showed greater stress and displacement under the modeled loading.

<img width="1467" height="651" alt="optimized_course_displacement(1)" src="https://github.com/user-attachments/assets/ce4e7c07-d092-4226-9617-319b0abda8ea" />
*Figure 14. Optimized crosshead — coarse-mesh displacement.*

<img width="1416" height="682" alt="optimized_course_stress" src="https://github.com/user-attachments/assets/485a6142-6b03-4d10-b333-5aa3db95febd" />
*Figure 15. Optimized crosshead — coarse-mesh von Mises stress.*

<img width="1388" height="615" alt="optimized_medium_displacement(1)" src="https://github.com/user-attachments/assets/4866785b-e6d3-493d-b2ab-e27ab33fb0d0" />
*Figure 16. Optimized crosshead — medium-mesh displacement.*

<img width="1404" height="695" alt="optimized_medium_stress(1)" src="https://github.com/user-attachments/assets/ca317488-87fe-4e9c-9b41-e5bc5951c738" />
*Figure 17. Optimized crosshead — medium-mesh von Mises stress.*

<img width="1374" height="627" alt="optimized_fine_displacement(1)" src="https://github.com/user-attachments/assets/eaa99f21-2774-4810-8e7b-de3c688c6e29" />
*Figure 18. Optimized crosshead — fine-mesh displacement.*

<img width="1384" height="614" alt="optimized_fine_stres(1)" src="https://github.com/user-attachments/assets/42a721dd-2ee8-4503-a754-6fc695eb5b12" />
*Figure 19. Optimized crosshead — fine-mesh von Mises stress.*

## Optimized design: mesh convergence check

I repeated the three mesh levels after removing material and adding fillets. The optimized mesh details recorded in SOLIDWORKS were 20,333 elements (coarse), 28,780 elements (medium), and 32,083 elements (fine), with zero distorted elements reported in each mesh.

| Mesh | Elements | Maximum von Mises stress (MPa) | Maximum resultant displacement (mm) |
|---|---:|---:|---:|
| Coarse | 20,333 | 4.283 | 0.003204 |
| Medium | 28,780 | 6.512 | 0.003227 |
| Fine | 32,083 | 6.136 | 0.003231 |

Medium-to-fine stress change = |6.136 − 6.512| / 6.512 × 100 = **5.77%**. Medium-to-fine displacement change = |0.003231 − 0.003227| / 0.003227 × 100 = **0.12%**. The displacement is stable across these refinements, while the maximum stress remains somewhat mesh-dependent. More local refinement at the highest-stress regions would help confirm stress convergence.

## Final measurements and percentage changes

After optimization, the mass dropped from 6.12 lb to 5.37 lb, which is a 0.75 lb reduction (about 12.25%). The volume decreased by 7.69 in³ (about 12.26%). The tradeoff was higher calculated stress and displacement in the fine-mesh results.

| Measurement | Original | Optimized | Change |
|---|---:|---:|---:|
| Mass | 6.12 lb | 5.37 lb | −12.25% |
| Volume | 62.74 in³ | 55.05 in³ | −12.26% |
| Fine-mesh maximum von Mises stress | 4.983 MPa | 6.136 MPa | +23.14% |
| Fine-mesh maximum displacement | 0.002185 mm | 0.003231 mm | +47.87% |

The simulation lists a yield strength of 275 MPa. Both reported fine-mesh maximum stresses are below that value for the assumed load and fixture conditions. This does not by itself validate the design for every operating condition.

## Factor of safety and design assessment

The SOLIDWORKS plots list a yield strength of 275 MPa. Using the fine-mesh maximum von Mises stress, the estimated yield-based factors of safety are:

- **Original:** 275 / 4.983 = **55.19**.
- **Optimized:** 275 / 6.136 = **44.82**.

The optimized part is lighter but shows increased maximum stress (about 23.14%) and resultant displacement (about 47.87%). The simulated load is carried from the center loading region toward the two restrained circular mounting regions, with bending visible around the center and arm transitions. Stress concentrations appear near transitions and mounting regions; the exact peak location and any change in that location should be verified using SOLIDWORKS probe results. The deformed shapes are highly exaggerated in the plots and do not, by themselves, quantify twisting or warping.

**Requirement still to verify:** The assignment calls for a 2 kN axial test load and maximum **vertical** deflection at the grip line. The supplied screenshots document the load direction and total resultant displacement (URES), but do not independently confirm the applied 2 kN magnitude or report the vertical displacement component at the grip line. These should be checked in SOLIDWORKS before claiming full compliance with the loading and deflection requirements. Likewise, final dimensional and stiffness constraints must be checked against the team's design requirements.

## Conclusion

The optimized crosshead uses less material and weighs about 12.25% less than the original. It also has higher simulated stress and displacement, so the weight savings come with a stiffness and stress tradeoff. I would verify the support and load assumptions and check mesh convergence before making a final design decision.

## Drawing

<img width="1206" height="782" alt="image" src="https://github.com/user-attachments/assets/7db661f3-7036-44c0-93d1-1d1e96371557" />


Downloads:
[CAD Files](Loose_Screws_A10_Downloads.zip)

