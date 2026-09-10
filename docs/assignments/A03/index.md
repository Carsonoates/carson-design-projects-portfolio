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

Once the model was extruded, I placed a fixture on the left side of the bar and attached the selected force on the right side. The force on the right side pulls on the bar, causing tension



## Decide


## Communicate

