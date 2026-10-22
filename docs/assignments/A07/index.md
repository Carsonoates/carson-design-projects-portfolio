# A7 – FEA on Bracket

## Objective
- Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.
- Ensure high stiffness, strength, and lightweight optimization through iterative design.
- Conduct multiple FEA simulations, refining geometry based on results.
- Perform static stress analysis, including constraints, loading, and meshing selection.
- Interpret data by identifying max stress, displacement, and safety factors.
- Optimize the design by modifying geometry to enhance performance.
- Document the entire process with images, calculations, and insights.
- Reflect on key engineering lessons learned and time spent.

## The Goal
For this assignment, I used FEA simulations to optimize the design of the bracket I created in previous assignments. The goal of this task is to make geometric changes based on the previous analysis results and create a high-stiffness, high-strength design that is as lightweight as possible. For convergence, our stress, displacement, and safety factor must fall within a 7% difference. The bracket I used for this assignment was the exact bracket I created in assignment A6.

## The Set-up
Before we start with the FEA simulations, we need to do some housekeeping to make sure this works properly. Since this is the previous design, most of the values have not changed, and the material is still A36 Steel. The things we need to add are fixtures, the applied load of 750 lbf, and mesh to the part. The mesh will change as the design process progresses, but for now I chose to use a coarse mesh for the first simulation.

<img width="222" height="154" alt="image" src="https://github.com/user-attachments/assets/0a0b7311-2dc3-4ef5-a9c3-f220e30024bb" />
<img width="372" height="227" alt="image" src="https://github.com/user-attachments/assets/44aca3e9-5404-4382-b921-021acf081baa" />
<img width="823" height="824" alt="image" src="https://github.com/user-attachments/assets/deba3432-d947-4802-b7a7-091705fd72be" />

# Loop #1 analysis

## The First Analysis
The first analysis came with a few expected outcomes and a few surprises as well. For starters, the displacement was reasonably large, as expected.
<img width="1133" height="1059" alt="image" src="https://github.com/user-attachments/assets/2542851d-e3d6-48e0-b2fb-921864a0161b" />


The stress was located in the area I figured it would be, but it had a higher value than expected.
<img width="1184" height="1072" alt="image" src="https://github.com/user-attachments/assets/2338132d-7782-4af7-95a4-53f2483d3ce2" />


The factor of safety, however, was incredibly low and very far off the factor of 4 I originally used in the design.
<img width="1134" height="1023" alt="image" src="https://github.com/user-attachments/assets/3e5a53af-5b80-47cb-8503-6c0f4a144def" />

To see whether this converges, we need to compare it with another analysis using the same settings but a finer mesh. The mesh used for this run falls in the middle of the two extremes, giving us a finer mesh than last while still leaving room for improvement. In this simulation, stress and displacement increased significantly, while the safety factor decreased substantially as well.

<img width="226" height="155" alt="Screenshot 2026-10-21 233228" src="https://github.com/user-attachments/assets/22ad3dd7-94bf-4ded-8603-752acafa17e6" />
<img width="411" height="272" alt="image" src="https://github.com/user-attachments/assets/fd3a8f9a-2843-4ff5-8510-4fba293f590f" />
<img width="869" height="804" alt="Screenshot 2026-10-21 233312" src="https://github.com/user-attachments/assets/7290c20b-fd6b-4bea-8674-a4c626241f68" />
<img width="1178" height="1071" alt="image" src="https://github.com/user-attachments/assets/b408aa52-52dc-4ab4-b91a-67e2d6debcfa" />
<img width="1177" height="1050" alt="image" src="https://github.com/user-attachments/assets/26ad0da5-fb7d-40fb-9335-4ac47120d7cf" />
<img width="1112" height="981" alt="image" src="https://github.com/user-attachments/assets/760a87ba-c3ec-4273-a4c1-f64eda2e21f1" />

Since the medium mesh did not converge, I ran another study using the finest mesh possible in SolidWorks.

<img width="227" height="158" alt="image" src="https://github.com/user-attachments/assets/378e7e1b-17d5-4615-98f0-2176e3230353" />
<img width="417" height="270" alt="image" src="https://github.com/user-attachments/assets/7eeea1e7-248d-423d-adb4-64a329134d48" />
<img width="1073" height="959" alt="image" src="https://github.com/user-attachments/assets/67949725-ec6a-4366-98cd-b523b15af599" />
<img width="1126" height="1025" alt="image" src="https://github.com/user-attachments/assets/3306f9d1-8a23-4d33-98f1-1e7e22d13f6f" />
<img width="1091" height="1017" alt="image" src="https://github.com/user-attachments/assets/381e019b-23dd-4f80-9387-9ee7af4fcfea" />
<img width="1126" height="977" alt="image" src="https://github.com/user-attachments/assets/cff09a3e-e04d-4427-827a-f96a63db1136" />

Here is the chart for the simulations for the first loop:

<img width="495" height="183" alt="image" src="https://github.com/user-attachments/assets/a0c729ed-2651-42e9-b876-a114ffbc0aa5" />


## Decide


## Communicate

