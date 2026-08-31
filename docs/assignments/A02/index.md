# A2 – Truss Stress Analysis

## Objective
The purpose of this project was to design a lightweight planar truss capable of supporting the loads specified in Figure 1. The truss members were designed using ASTM A500 steel, using hardened tool steel coonection pins. 
The requirements for this assignment was selcting truss geometry, calualtions support reactions and internal force members and creating a fianl CAD model.
## Analyze


- Initial Truss drawing 

![Truss Sketch](Screenshot%202026-08-27%20164238.png)
-
-  Intial Truss Drawing with Dimensions

![Truss Sketch](TRUSS-DIMENSIONS.png)

The truss has a total horizontal distance of 1.2 m, divided into three 0.4 m sections, with a vertical height of 0.3 m. From this geometry, the outside diagonal members form an angle of approximately \(36.87^\circ\). The applied loads at C and D each have a magnitude of 25 kN but act in opposite vertical directions.

-Support Reactions and INTERNAL FORCE MEMBERS 

![Truss Sketch](SUPPORT-REACTIONS.png)

IN order for me to find the individual truss memeber i first find Ax and Ay which is the external forces at the support. After finding thr external forces I drew a free-body diagram of the entire truss and used the equilibrium equations and the moments equations and setting them equal to zero to find them. 

From my calculations, I obtained:

$$ A_x=0 $$ $$ B_y=8.33\text{ kN} $$ $$ A_y=-8.33\text{ kN} $$

The negative sign for \(A_y\) means that its actual direction is opposite to the direction I initially assumed on my free-body diagram.

INTERNAL FORCE MEMBERS



![Truss Sketch](JOINTa,b.png)

![Truss Sketch](JOINT-E.png)

After finding the support reactions, I used the method OF JOINTS to find all the others forces in each memeber by using \(\Sigma F_x=0\) and \(\Sigma F_y=0\) to solve the forces directly. I assumed unknown member forces were in tension initially, and a negative result indicated that the member was actually in compression.

At Joint B, I used the \(36.87^\circ\) angle and the previously calculated reaction force to solve for members BC and BE. My calculations gave:

$$ F_{BC}=-13.88\text{ kN} $$

so BC is in compression, and

$$ F_{BE}=11.11\text{ kN} $$

so BE is in tension.
After solving all the internal members, I found out that  $$ 20.03\text{ kN}. $$. This was the largest internal force in my truss, so this will be used  \(20.03\text{ kN}\) as the critical load when sizing the truss members.

Truss Member Cross-Sectional Area

![Truss Sketch](AREA.png)that the 

After determining all of the internal forces, I needed to find a cross-sectional area that would prevent the truss members stress from going to or pass the yield strength. The yield is the point where the materaisl will no longer go back to original shape after it had been stretch or defrom. we Dont want that in ourtruss desgin so I used the largest internal force of \(20.03\text{ kN}\). I sue the largest force member because designing the beam using the largest force member will ensure the otehr smaller forced members will be safe. 

As show the using the factor of safety and the allowable stress the minimum area for the truss is Solving symbolically for minimum area gives 
	​

- 

## Decide


## Communicate

