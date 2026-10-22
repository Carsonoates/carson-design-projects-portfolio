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

## FEA Simulations
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

Since the medium mesh did not converge with 49.1%, 55.6%, and 48.8% for stress, displacement, and safety factor, respectively, I ran another study using the finest mesh possible in SolidWorks.

<img width="227" height="158" alt="image" src="https://github.com/user-attachments/assets/378e7e1b-17d5-4615-98f0-2176e3230353" />
<img width="417" height="270" alt="image" src="https://github.com/user-attachments/assets/7eeea1e7-248d-423d-adb4-64a329134d48" />
<img width="1073" height="959" alt="image" src="https://github.com/user-attachments/assets/67949725-ec6a-4366-98cd-b523b15af599" />
<img width="1126" height="1025" alt="image" src="https://github.com/user-attachments/assets/3306f9d1-8a23-4d33-98f1-1e7e22d13f6f" />
<img width="1091" height="1017" alt="image" src="https://github.com/user-attachments/assets/381e019b-23dd-4f80-9387-9ee7af4fcfea" />
<img width="1126" height="977" alt="image" src="https://github.com/user-attachments/assets/cff09a3e-e04d-4427-827a-f96a63db1136" />

Here is the chart for the simulations for the first loop:

<img width="497" height="182" alt="image" src="https://github.com/user-attachments/assets/08a15392-391f-48d9-b3eb-84a6f1ba819f" />

# Loop #2
For this loop, I increased the thickness of feature B from .10 to .30 in, added .25 in fillets on the outside edges, and shortened the height of feature E.
<img width="1109" height="966" alt="image" src="https://github.com/user-attachments/assets/545b73e9-6f87-4aef-8461-6d6deecef89d" />

## FEA Simulations: Part 2
The hope here is that the changes I made to the top of the bracket remain as uninvolved as they were in the original design, while the increased thickness of feature B provides more support against stress and displacement. Following a similar setup to the previous loop, I started with a coarse mesh and planned to work up from there.

<img width="228" height="159" alt="image" src="https://github.com/user-attachments/assets/d533a1b5-ff28-40a0-aeee-170ca0b792dd" />
<img width="416" height="275" alt="image" src="https://github.com/user-attachments/assets/7833ec7e-6056-4dd5-b634-d8daf0d0b443" />
<img width="1088" height="999" alt="image" src="https://github.com/user-attachments/assets/82ed07cd-b424-4240-8343-adcc2c1ff13d" />

Running the first simulation shows that my assumptions about the changes I made were correct, but to my dismay, the changes to the problem area weren't affected as much as I would've liked. The top of the bracket remains steady despite shaving off a good bit of material, yet the bottom still requires some more attention. Nevertheless, it was still an improvement to the design

<img width="1145" height="1068" alt="image" src="https://github.com/user-attachments/assets/03057b1f-8e89-4c21-9f7c-c46d6dd4b438" />
<img width="1137" height="1012" alt="image" src="https://github.com/user-attachments/assets/3812fd8e-f341-4a73-8100-65bc234185c0" />
<img width="1130" height="1006" alt="image" src="https://github.com/user-attachments/assets/e88f9e63-ba84-4bd5-9ffa-8c761438cca4" />

The next step was to start refining the mesh and run the simulation again.

<img width="376" height="264" alt="image" src="https://github.com/user-attachments/assets/85b79143-cdfd-4214-bbf5-ff82504e139d" />
<img width="855" height="808" alt="image" src="https://github.com/user-attachments/assets/fc1b350b-cb33-47a5-8cd0-546b4eb4af61" />
<img width="1210" height="1007" alt="image" src="https://github.com/user-attachments/assets/d3685437-f527-4c5f-b3e5-3c0fa8cfb018" />
<img width="1249" height="973" alt="image" src="https://github.com/user-attachments/assets/129de11a-dc92-4b35-9907-6eda21445470" />
<img width="1269" height="996" alt="image" src="https://github.com/user-attachments/assets/3acd8881-8e7c-4c93-b870-c18e232014df" />

Since the medium mesh did not converge with 23.4%, 9.6%, and 23.6% for stress, displacement, and safety factor, respectively, I ran another study using the finest mesh possible in SolidWorks.

<img width="370" height="228" alt="image" src="https://github.com/user-attachments/assets/bc38fb1b-5e32-4d2d-a030-47c3aa22a432" />
<img width="1117" height="964" alt="image" src="https://github.com/user-attachments/assets/abd57167-f6f2-42ee-8843-1ac8ab463300" />
<img width="1246" height="1050" alt="image" src="https://github.com/user-attachments/assets/e5373750-b6aa-4fc0-8a45-f8506627ecbc" />
<img width="1188" height="1026" alt="Screenshot 2026-10-22 013211" src="https://github.com/user-attachments/assets/b3fdea45-274c-4796-9855-f3195551c3eb" />
<img width="1171" height="1018" alt="Screenshot 2026-10-22 013242" src="https://github.com/user-attachments/assets/40d8d736-c23b-4632-8c2d-5cf3c2732c34" />

Here is the chart for the second loop:

<img width="496" height="186" alt="image" src="https://github.com/user-attachments/assets/ff4f9f77-8776-41e3-a440-5c40ddd17bac" />

# Loop #3
For the third loop, I shortened the total length of the top bracket by 1 in. For the problem area, which is feature B, I added another .05 in to the thickness and added triangular extensions to the sides.

<img width="965" height="993" alt="image" src="https://github.com/user-attachments/assets/60625f17-9fe1-4f23-8170-26aceda53ce4" />

## FEA Simulations: Part 3
Once again, I prepared the model for analysis. With the first sim done, it seems I shaved a bit too much off the top of the bracket, but I did manage to strengthen the problem area enough to fit within the boundaries of the material

<img width="371" height="285" alt="image" src="https://github.com/user-attachments/assets/69a3b74a-5e37-4a71-864f-f8b63586ece2" />
<img width="966" height="1030" alt="image" src="https://github.com/user-attachments/assets/441ee6f1-342b-4639-84b6-565b445ceed0" />
<img width="1131" height="1016" alt="image" src="https://github.com/user-attachments/assets/e2afc790-12ab-43a0-b995-88342a117d84" />
<img width="1075" height="1021" alt="image" src="https://github.com/user-attachments/assets/b72e0443-b138-40c6-94cd-100d8bf31dae" />
<img width="1094" height="1019" alt="image" src="https://github.com/user-attachments/assets/a161e553-134e-44f3-9926-c6bce5affe69" />

Preparing the second sim:

<img width="369" height="229" alt="image" src="https://github.com/user-attachments/assets/79e108d4-f4f1-4e0a-baac-723f873c59c7" />
<img width="971" height="999" alt="image" src="https://github.com/user-attachments/assets/20fead71-28ac-48fc-a06e-cfcd861fb852" />
<img width="1055" height="1016" alt="image" src="https://github.com/user-attachments/assets/e83e66fe-6744-4c33-a4ef-b46a53302a87" />
<img width="1088" height="1037" alt="image" src="https://github.com/user-attachments/assets/b232d89f-5306-4e9c-971b-c73976d3321b" />
<img width="1006" height="1022" alt="image" src="https://github.com/user-attachments/assets/6b232697-a1f0-4f66-b565-08ad21be6ed3" />

Since the medium mesh did not converge with 20.5%, 5.6%, and 20.7% for stress, displacement, and safety factor, respectively, I ran another study using the finest mesh possible in SolidWorks.

<img width="370" height="193" alt="image" src="https://github.com/user-attachments/assets/6b9f816f-ce50-4dfe-86a5-4ee078581502" />
<img width="958" height="1004" alt="image" src="https://github.com/user-attachments/assets/14f729a1-72b4-4d3a-9aa4-8c8dde98a945" />
<img width="1007" height="1020" alt="image" src="https://github.com/user-attachments/assets/527bd513-be6f-4128-82d5-16a085c4e4c8" />
<img width="1105" height="1026" alt="image" src="https://github.com/user-attachments/assets/97f9cfa5-0080-4488-8921-bd76eab1f0cd" />
<img width="1014" height="1016" alt="image" src="https://github.com/user-attachments/assets/3e2e5bdf-1bb7-450a-834e-e510bd4a9290" />

Here is the chart for the third loop:

<img width="494" height="182" alt="image" src="https://github.com/user-attachments/assets/ac29417a-626c-4fca-ae07-c5827b1ad2a9" />

# 2157 The Link



