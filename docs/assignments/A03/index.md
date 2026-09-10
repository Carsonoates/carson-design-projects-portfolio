# A3 – Parametric and FEA

## Objective
- Use axial deflection modeling to design its dimensions
- Use parametric design to determine a bar's length
- Introduce FEA (Finite Element Analysis)
- Introduce linking dimensions to appropriate parameters in CAD.
- Compare and contrast the different analysis


## 1. Designing the Bar
### a.
For this assignment, I was told to design a bar parametrically. The bar's design must include a circular cross-section, a max axial deflection of 0.009 inches, an applied direct load of 300lbf to 500lbf, and must be made out of aluminum. For the cross-section, I chose a diameter of 0.5 inches, and I set the applied load to 400 lbf. I researched aluminum properties to find the appropriate Young's Modulus, which I found to be 9.86 x 10^6 psi and falls within the range I was given (source found [here](https://www.matweb.com/search/datasheet.aspx?bassnum=AMEAL00&ckck=1)). With the necessary values now set, I first found the bar's area using the equation provided here: A = (pi * d^2) / 4. 
<img width="723" height="229" alt="image" src="https://github.com/user-attachments/assets/26d97c7a-3dc2-40dd-a354-0845995339df" />

### b. 
Now that we have the idea of what our bar will look like, we need to find our bar's length. We can find this value using the tension elongation equation found in the Machinery's Handbook: e = FL / AE, where e represents elongation. By rearranging this equation and replacing A with our previously found area equation, we find our parametric equation L = (e E pi d^2) / 4F.

<img width="303" height="233" alt="image" src="https://github.com/user-attachments/assets/3c230db8-0de3-4374-a86c-fadb8ce67d07" />

### c.
With everything now defined and our equation found, we can begin the CAD model. Starting it all off, I first input our variables into SolidWorks using the equations feature.
<img width="2310" height="294" alt="A3 Equations" src="https://github.com/user-attachments/assets/a21aed85-5132-4742-830a-620c0edef3cc" />

Using these, I drew a sketch of a circle and set the diameter to the variable "d".
<img width="671" height="580" alt="A3 Sketch" src="https://github.com/user-attachments/assets/8bb8219b-aab0-49b3-bf79-a9c5ac0d23cf" />

Then I extruded the model outward with the length found using the parametric equation.
<img width="1743" height="543" alt="A3 Extrude" src="https://github.com/user-attachments/assets/39b3b43c-8193-4824-8a35-ddd412c34eee" />

Once the model was extruded, I placed a fixture on the left side of the bar and attached the selected force on the right side to add tension to the FEA analysis. With the fixture and the force now applied, I changed the material to the required aluminum properties I was directed to add. However, SolidWorks does not have aluminum as a material in its basic database, so I created the material using the values I found through research to mimic aluminum as closely as possible. The last requirement to start the simulation was to add a mesh to the model.

<img width="703" height="515" alt="A3 Fixture" src="https://github.com/user-attachments/assets/bd25d2ca-8dfb-4190-bc92-a34a8b89e13e" />
<img width="1094" height="748" alt="A3 Force" src="https://github.com/user-attachments/assets/ba3c659b-2196-497c-9bcf-1593634caf21" />
<img width="1524" height="901" alt="A3 Mesh" src="https://github.com/user-attachments/assets/f8a84c45-ab38-4b2e-a053-f3a754a4b121" />
<img width="812" height="575" alt="A3 Material Properties" src="https://github.com/user-attachments/assets/494114db-61cc-401a-8bf4-ed99eab93037" />


## 2. FEA Analysis
### a/b. 
Using SolidWorks' simulation feature, I generated two maps with the settings I applied to the bar model. The first map displays the deflection across the entire bar, and the second shows the stress across the model. With the measurements from the maps, I found the max stress applied to be 2166 psi and the max deflection to be 0.009008 inches.
<img width="1438" height="795" alt="A3 Deflection" src="https://github.com/user-attachments/assets/9293b490-cc2f-4b0a-881e-5860f5d56064" />
<img width="1485" height="765" alt="A3 Stress" src="https://github.com/user-attachments/assets/78b2dbdf-e67f-411b-9ad5-1268d92dce8d" />

### c.
With these measurements, I calculated the safety factor of the bar using the ratio of aluminum's yield strength to the maximum stress applied to the bar, which came out to be a factor of 18.

<img width="594" height="280" alt="Screenshot 2026-09-09 214501" src="https://github.com/user-attachments/assets/ed2a3e2e-6fab-413d-8891-3259fe4589ed" />

## 3. Design Reflection

### a.
For the axial deflection, I found the difference between my calculated value and the measured value to be extremely small, with the percentage difference being only 0.08%.
<img width="337" height="225" alt="Screenshot 2026-09-09 214506" src="https://github.com/user-attachments/assets/aec133ec-061d-4e94-868c-133864d37820" />
<img width="543" height="189" alt="Screenshot 2026-09-09 214510" src="https://github.com/user-attachments/assets/86477956-e74b-4cdc-ad38-9e071dcfcdc6" />

**i.** I didn't find any big discrepancies in these values. While my calculated value is smaller than my measured value, it's such a tiny difference that I believe both values could be used interchangeably. **ii.** This makes sense to me due to the test's simplicity. Applying only one load in one direction that causes the smallest deflection on a solid body makes little room for great changes. **iii.** In the end, I still believe that the hand calculations are more trustworthy than the simulation. Technology has become much more advanced and is growing more and more each day. However, the equations used to find these have been used for much longer and have been proven to be reliable time and time again.

### b.
As a small extra, we were instructed to use our imaginations. I was to imagine a small hole on the left side of the bar, the side that was fixed, and to find the peak stress located at that hole and determine if it would still pass the safety factor. First, I found the stress concentration factor for a round bar undergoing tension using the equation listed here: d / D, where d represents the hole diameter, and D represents the bar's diameter. Using the chart and a hole diameter of 0.2 inches, I discovered my concentration factor to be 4.4.

<img width="675" height="309" alt="Screenshot 2026-09-09 214514" src="https://github.com/user-attachments/assets/97f5d89a-719a-4168-a27a-1df29dd0a65e" />

## 4. What I learned from this assignment
This assignment has shown me two main things. The first is related to engineering principles. With this task, I have discovered how simulations can show a correlation between the physical properties of an object or model and the equations and calculations used to design the model. The second lesson is to always make sure you have everything needed to complete a project ahead of time. I realized halfway into this assignment that I was missing the software required to run the simulation necessary for step 2. Thankfully, I learned my lesson from the last assignment and started early in the week, which gave me ample time to find and install the necessary software.

The assignment was completed in 3-4 hours.

## 2157 Problem

<img width="510" height="213" alt="Screenshot 2026-09-09 232004" src="https://github.com/user-attachments/assets/1a26b529-6740-48d1-8853-e764c0d10389" />

SolidWorks Download: [Download Bar.SLDPRT](./BarCMO.sldprt)

