# A5 – [Topic]

## Objective


## Analyze
##  Stress Analysis
### Feature A

![A3](A_1.png)
Feature K is to support the polyester strap that applies the horizontal load to the rigid T-beam. For this design I selected an applied force of 600 lbf, which meets the problem requirement of 500<F≤800 lbf. The strap is pulling on both sides of Feature K, so the total load on the feature is twice the force applied. The total load used in the analysis is thus W=2F=2(600)=1200 lbf

The bracket was made of Aluminum 6061-T6 material. The analysis was performed with the yield strength of approximately 35,000 psi. The safety factor for the assignment is 4.
The material selected is Aluminum 6061-T6.

The biggest unknown is the smallest radius for Feature K. The first step in determining the radius is to find out the minimum required section modulus. Once the minimum radius is identified, the minimum diameter of the cylindrical feature can be determined using D=2R
for the assumption It is assumed that feature K is not failing in direct shear as specified in the assignment for this analysis. The polyester strap is assumed to exert two equal forces on the feature, resulting in a total force of 2F. The strap load is modeled as a distributed load along Feature K.

Feature K is modeled as a beam of constant solid circular cross section. The material is taken to be linearly elastic up to the yield point. The first sizing calculation ignores stress concentrations around the ends of the feature.

![A3](A_2.png)
The free-body diagram for Feature K shows the cylindrical member supporting the load from the polyester strap. 
The maximum bending stress equation provided in the assignment is σmax​=2ZWL​ and The allowable stress is determined by dividing the yield strength by the safety factor is σallow​=SFSy​. For the design to satisfy the required safety factor, the maximum bending stress must not exceed the allowable stress so WL/2Z=Sy/Sf and Z. 
Feature K is designed with a solid circular cross section. The moment of inertia for a solid circular member is I=πr4​/4. The section modulus is defined as Z=I/r, then I Substitute the moment of inertia equation to get r. 

​

![A3](A_3.png)


### Feature B

![A3](A_4.png)
For Feature B, I used the reaction force calculated from Feature A as the applied load. Since Feature A is supported symmetrically, the total 1200 lbf strap load is divided equally between the two supports. This gives an applied load of 600 lbf on each Feature B.

So here's what went down with Feature B—we treated it like an axially loaded member. The force coming from Feature A pushes down on Feature B, and the bracket's other parts push back up with equal force. We neglect direct shear failure (like the assignment said) and didn't worry about stress concentrations at the joints for the initial sizing. Pretty straightforward.

We went with a safety factor of 4 to keep things nice and safe, making sure Feature B stays below the yield strength of Aluminum 6061-T6.

I pulled Feature B out from the rest of the bracket setup to draw up the free-body diagram. So here's what's going on: Feature A is pushing down on Feature B with a force of 600 lbf at its bottom end. Meanwhile, the upper part of the bracket is pushing back up with a reaction force to balance things out.

![A3](A_5.png)
Since Feature B acts like an axially loaded member, I went with the standard normal stress formula: σ=P/A. 
To find the allowable stress, you take the material's yield strength and divide it by your safety factor:
σallow​=Sy/FS
When you're looking for the smallest cross-sectional area that'll work, I set the normal stress equal to the allowable stress and solve for the minimum area​. which comes out to be 0.0686 in^2​. 
Since Feature B has a rectangular cross section: A=wt, the selected width and thickness must satisfy 0.0686 in^2. Using that logic i found out that the min thickness is 0.137 in

### Feature c
![A3](B_1.png)
For Feature C the load came from the previous part so the lower section could handle the bending. It needed to keep the safety factor at 4 under that 600 lbf. The numbers used were the load itself, the factor of safety, and the yield strength at 35000 psi. The bracket material was Aluminum 6061 T6. For the analysis, I used: P_C=600 lbf, FS=4, S_y=35,000psi. The material selected for the bracket was Aluminum 6061-T6. The length of Feature C was determined from the dimensions of the rigid T-beam. The main values I needed to determine were the minimum section modulus and the minimum height of Feature C. 

For the assumption of this analysis, it is assumed that the load from Feature B is transferred to the right of Feature C and forms a moment due to the transfer of load. It is also assumed that the left end of Feature C is the resisting connection that offers both vertical reaction and moment reaction.
Another assumption made for this analysis is that direct shear failure can be ignored, as per the assignment. Stress concentration due to corners and connections is ignored initially for the calculation of strength, and the cross-sectional shape of Feature C is considered rectangular.

For the FBD Feature C was separated from the remaining bracket structure. There is a load of 600 lbf applied vertically to the right of the feature. To the left of the feature, there is a reaction force R_c and a moment M_C.

![A3](B_2.png)
FOr the algebraic solution, I used moment equilibrium about the left side of Feature C: ∑Mleft​=0, to get the largest bending moment occurs at the resisting end as MC​=PC​LC. To determine the required section size, I used the bending stress equation σ=M/Z, the allowable stress σallow​=Sy/FS and setting them equal to solve for Zmin. For the rectangular cross section, I used: Z=(Wc*h^2)/6 as the section modulus to solve for the hmin​. ​​​​​


![A3](B_3.png)

FOr the Numerical Bending Moment i use PC​=600 lbf, LC​=2.4964 in, to solve for the Mmax the maximum bendding moment. Next, I calculated the minimum required section modulus as 0.1712 in , this means Feature C needs a section modulus of at least: 0.1712 in. 
Then for the Minimum Height of Feature C Using the rectangular section modulus equation Z=Wh^2/6, and Using the width adopted in my calculation  I solved for the minimum height of 0.6415in. 


##  Stifness Analysis


![A3](B_4.png)

![A3](B_5.png)

![A3](B_6.png)

![A3](B_7.png)

![A3](B_8.png)

![A3](B_9.png)

![A3](B_10.png)

![A3](B_11.png)

![A3](B_12.png)

![A3](B_13.png)


## Decide


## Communicate

