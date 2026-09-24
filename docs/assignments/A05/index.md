# A5 – [Topic]

## Objectives
- Conduct stress analysis to determine appropriate dimensions for structural features.
- Generate free-body diagrams (FBDs) to visualize forces and constraints for each feature.
- Identify and document known and unknown variables, assumptions, and algebraic models for stress calculations.
- Perform stiffness analysis to establish minimum required dimensions based on deflection constraints.
- Compare stress and stiffness analyses to ensure structural integrity and compliance with given constraints.
- Create detailed multiview sketches illustrating dimensions derived from both stress and stiffness analyses.
- Reflect on and document key engineering lessons learned throughout the process.

## Starting Out

For this assignment, I was told to design a bracket using the following given parameters.

<img width="868" height="654" alt="image" src="https://github.com/user-attachments/assets/38574378-288c-471c-883a-94ca0c1d678b" />

To start this assignment, I began writing general sketches and notes I thought would be useful for the rest of the project, starting with the chosen load value of 750 lbf. I then wrote down all of the knowns I was given and that I found through research on [A36 Steel](https://www.azom.com/article.aspx?ArticleID=6117), my chosen metal, and its important values. I also wrote down some basic universal assumptions along with a sketch of the bracket concept design.

<img width="1044" height="396" alt="image" src="https://github.com/user-attachments/assets/e7ee5c7b-593b-4ee4-91a2-a5544a458f21" />

## Stress Analysis Design Process

With all the setup now finished, I began solving for the dimensions of the bracket using stress as the basis for them. I found it to be easiest if I started with the bottom feature of the bracket I labeled as feature A. Using the known values and the listed assumptions, I began solving for the unknown value of feature A. For this feature, I needed to find the diameter of the cylindrical beam that would hold the given polyester strap we were to use as a reference. By treating the feature as a cantilever beam, I was able to find a diameter of .858 in., which I rounded up to .875 for simplicity. Using the force value from A and the diameter we just found, I moved on to Feature B, which was treated as an axially loaded bar, simplifying the process. For this feature, I needed to find the thickness using the previous values I found in Feature A. With these, I found the value of B's thickness to be .094 in., which was rounded to .125 for verification. This process continued for each feature in line until I was able to fully define the bracket's design.

<img width="1046" height="917" alt="image" src="https://github.com/user-attachments/assets/1527cb3a-3ea9-4a2a-afee-306ea1b96c9d" />

Feature C was defined by treating it as a beam supported on both ends with a load in the center. The unknown I found for C was its height, which came out to be .352. This was then rounded up to .360 for a comfortable clearance in the verification.

Feature D, when the unknown was solved for, ran into a problem. The found value of the base was originally .275; however, this does not clear the verification. This problem was dealt with when I rounded the value to .325. I believe the issue with the calculation was originally rounding the value to .275 instead of using the full value given by the equation.

<img width="911" height="268" alt="image" src="https://github.com/user-attachments/assets/61e088be-9fb3-498e-ae6e-56c711d18857" />

I then ended the analysis with Feature E by treating it as a cantilever with a distributed load to find the unknown height to be .787, rounded to .8 for simplicity.

<img width="992" height="207" alt="image" src="https://github.com/user-attachments/assets/80732365-f26c-4615-a6bd-b4e52bc2daf6" />

## Stress Analysis Design Multiview

The next task was to draw out a multiview of the final design of the bracket.

<img width="472" height="454" alt="image" src="https://github.com/user-attachments/assets/8c958a2c-6245-4332-a0ba-6927959253cd" />

## Stiffness Analysis Design Process

Now it's time to follow the same process, but design for stiffness instead of stress. This follows similar assumptions, knowns, and unknowns as the stress analysis, so it was just a matter of finding the right equations and values to use for each feature. Then, to follow through the bracket, using the previous values to solve the next feature.

<img width="1013" height="274" alt="image" src="https://github.com/user-attachments/assets/a3d8a0a1-1695-4ce7-8cc4-d439364f102a" />

<img width="1028" height="233" alt="image" src="https://github.com/user-attachments/assets/e6188586-f8dd-4d0f-ada3-9bc3895cd156" />

<img width="1006" height="281" alt="image" src="https://github.com/user-attachments/assets/b5f95261-e7dc-411a-ab52-c658070656d4" />

<img width="1012" height="265" alt="image" src="https://github.com/user-attachments/assets/7e239b07-8931-487a-b1d0-0592a080e97b" />

<img width="890" height="291" alt="image" src="https://github.com/user-attachments/assets/bb114150-e133-4761-a0fd-ea84ba788259" />

## Stiffness Analysis Design Multiview

Then I created a multiview drawing of the stiffness version of the bracket with the newly found dimensions.

<img width="373" height="348" alt="image" src="https://github.com/user-attachments/assets/bf1bf358-16b0-4c38-9b72-7846d65b60ed" />

## Governing Failure mode:

By finding the dimensions for both stress and stiffness, the designs above feature only the values found in their respective section. In a proper design, the best values to use are the largest of the two values when compared. For Feature A, designing it for stress is the better option, as it is much larger than its stiffness counterpart, with stress requiring .875 and stiffness requiring .459. For Feature B, designing for stress is the better choice, with stress requiring 0.094 and stiffness requiring 0.0044. Feature C will also be designed for stress, with a .08 difference. Feature D is going to be designed for stress, with stress requiring 0.275 and stiffness requiring 0.048. Feature E goes in stress's favor, with stress requiring .787 and stiffness requiring .545.

## Error Propagation

I could not find an error in the propagation in the entire assignment. I believe I managed to catch the issue of failing to account for symmetry before it spiraled out of control.

## Assumption Sensitivity

One Assumption I would have changed for this project is the assumption I made for Feature D in the stress analysis. I think that if I treated the feature as a cantilever instead, the original value would have fit within the required safety factor.

## 2157 Only: Fits

### 1.

Since I'm in 2157, I'm subjected to more work. This time around, I was to design a link to connect feature A to a 1-inch shaft. The hole for Feature A was to allow a running/sliding fit, and the hole for the 1-inch shaft was to be designed with light assembly pressure or a light drive fit. To start, I calculated the smallest cross-sectional holes using stress and deflection equations.

<img width="776" height="266" alt="image" src="https://github.com/user-attachments/assets/83bdc706-6576-4522-8b21-94b6282d0c00" />

### 2.

The next step was to find the proper hole to use for the running/sliding fit. For this, I decided that an RC2 H6 hole was the best option for this fit. The process would be rounded out using a reamer. The tables used for this are shown here.

<img width="1237" height="758" alt="Screenshot 2026-09-24 024339" src="https://github.com/user-attachments/assets/d43dba30-61e9-4fe9-9e80-195951be84b4" />

<img width="1233" height="709" alt="Screenshot 2026-09-24 024757" src="https://github.com/user-attachments/assets/91df880c-e895-4267-b6fd-8d944883b21b" />

### 3. 

For the 1-inch shaft, I found the FN1 H6 option to fit best for this process. Reaming would be used to match the proper hole size. The tables used for this are shown here.

<img width="1213" height="695" alt="Screenshot 2026-09-24 024513" src="https://github.com/user-attachments/assets/b24365a7-c99d-4cec-a530-b8579bb3677d" />

<img width="1229" height="706" alt="Screenshot 2026-09-24 024727" src="https://github.com/user-attachments/assets/89a1dffb-b841-44e6-9947-b0f244fbcb74" />

## Lessons Learned

From this assignment, I learned how to take values from certain parts of a project and translate them throughout the rest of the design. I also learned how to use context clues when designing a part or feature to help fill in missing variables.

This assignment took me 7 hours to complete.
