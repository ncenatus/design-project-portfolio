# A5 – [Topic]

## Objective


## Analyze

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

## Decide


## Communicate

