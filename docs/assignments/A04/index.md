# A4 – [Topic]

## Objective
The objective for this project was to design a motor mount for a 24 V DC gear motor that bolts onto a rigid wall. Since the motor shaft puts out about 300 N of force, the mount needed to be tough enough to resist bending without yielding or sagging more than the 0.30 mm limit. I went with ABS plastic and stuck to the required safety factor of 3.

I broke the design down into two parts: Feature 1 holds the motor, and Feature 2 handles the wall connection. Once I finished the beam bending math, I took those dimensions and built a parametric 3D model in Creo.

## FEATURE 1 

![A3](A.png)
This is the calculation of the maximum stress equation for this assignment. I used the beam bending stress equation and the moment of inertia for a rectangular corss-section to caluclate the maximum stress equation. 
After that  I sketched out a free-body diagram. The 300 N motor force pulls down on the free end of Feature 1, which creates reaction forces and a moment at the fixed end. Since the maximum bending moment happens right at that fixed end, that's the spot I focused on to figure out how thick the mount needed to be. I calculated the max moment for the cantilever and then plugged that number straight into the bending-stress equation.
![A3](A_1.png)

FOr the design to be safe, the actual stress must be greater or equal to the allowable stress. Using the allowed stress and actual stress i then solve solve for the hyield. The hyield is the minimum thickness that the beam must be so that it does not exceed the allowable bending stress. 
The i solve for hd. The hd is the minimum thickness that the beam can be so that it don't pass the maximum allowed deflection of 0.3mm. I used the maximum delfection for a cantilever beam with a concentrated point load equation, then i substitute the moment of inertia equation to solve for the hdeflection. 
The Sy is the tensile strength of ABS material which is 29.6 MPA.

![A3](A_2.png)
Once I verified the yielding, I moved on to checking the deflection. I used the standard cantilever-beam equation for an end load, substituting in the moment of inertia for a rectangular cross-section to solve for the thickness. When I ran the numbers, the deflection limit called for a minimum thickness of about 17.50 mm.

Since 17.50 mm is thicker than the 13.51 mm required for yielding, the deflection requirement was the real deciding factor for the design. I ended up choosing 18.5 mm for the final CAD model. I went with that size because it covers both minimums and gives me a bit of extra breathing room without making the whole mount too bulky.

## FEATURE 2

![A3](A_3.png)

Feature 2 is the vertical part of the mount that actually bolts onto the wall. It has to handle the bending moment passed over from Feature 1, so I used beam-bending equations for this part of the model too. Just like with the first feature, it had to be strong enough not to yield and stiff enough to stay under the deflection limit. 



![A3](A_4.png)
The weight and load on Feature 1 create a moment that has to pass through Feature 2 to get to the wall. Because of that, I went back to the standard bending-stress formula to figure things out. For a rectangular cross section like this one, that simplifies down to a specific equation for maximum stress. By plugging in the yield strength for ABS and applying the safety factor of 3, I was able to solve for the smallest thickness I could get away with. After running the numbers, it looks like I need at least 13.5 mm to keep the material from yielding.

The yield calcualtion was a minimum required thickness of 13.5 mm, while the deflection calculation had a minimum thickness of approximately 14.45 mm. Since the deflection requirement controlled the design, so i can only choose a h value that is highher than both of them.  I selected a 15 mm thickness for Feature 2 so that both the yield and 0.30 mm deflection requirements were satisfied.


## ISOMETRIC VIEW 
![A3](A_8.png)
I started out by drawing an isometric sketch of the motor mount before I even touched the CAD software. This really helped me figure out the connection between Feature 1 and Feature 2, not to mention finding the right spots for the motor and wall mounting holes. I made sure to pull in the dimensions from MY calculations, so the sketch worked as a solid roadmap once I got into the solid works model.

For the main specs, Feature 1 ended up at 40 mm long and 18.5 mm thick. Feature 2 had a height of 30 mm and a thickness of 15 mm, with the whole thing coming in at a width of 40 mm.

## CAD DRAWING


### Step 1 – Creating Parametric Dimensions

![A3](A_5.png). 
When I started the solidworks model, I decided to set up parameters for all the main dimensions rather than just typing them in one by one. I set these up for things like the total width, the lengths and thicknesses for both Feature 1 and Feature 2, plus the shaft clearance and bolt-hole diameters. 

Going this route makes the whole model a lot more flexible. If I need to change something, I just update the parameter and the geometry follows suit. Plus, the assignment actually called for parametric modeling wherever it made sense, so this kept me on track with those requirements.

### Step 2 – Creating Feature 1

![A3](A_6.png)
I first created the horizontal motor-support section. I sketched the rectangular profile for Feature 1 and used the Extrude command to create the solid geometry.

The calculated minimum thickness based on deflection was 17.50 mm, but I used 18.5 mm

for the extrusion thickness. This ensured that my CAD geometry remained above the analytical minimum.


### Step 2 – Creating Feature 2
![A3](A_7.png)

After that, I moved on to the vertical wall-mounting section. I drew the sketch for Feature 2 so it was perpendicular to Feature 1, then extruded it out to match the full width of the mount.

The math for the deflection suggested I needed about 14.45 mm, so I ended up going with a final thickness of 15 mm. I also stuck with the 30 mm height I had picked out earlier. In the end, it turned into one solid L-shaped part instead of a bunch of separate pieces.


### Step 3 – Creating the Motor Clearance

![A3](A_9.png)

![A3](A_11.png)


![A3](A_10.png)

Once Feature 1 was done, I pulled the motor specs from Appendix A to figure out exactly where the shaft and mounting holes needed to go. The motor has this 22 mm locating feature on the front, so I worked right off the drawing instead of just guessing the size or placement of the opening.

I drew the circles on the top face of Feature 1 and then used an extruded cut to clear out the material. This gave me the room I needed for the motor and shaft while making sure everything stayed perfectly centered on the mounting surface.

### Step 5 – Creating the Wall Bolt Holes

![A3](A_12.png)

![A3](A_13.png)

Since the assignment called for bolt clearance holes, I went with a 3.4 mm diameter for the wall mounts. 

I started by placing one 3.4 mm hole on the vertical wall and set it 7.5 mm away from the edges. Once that was locked in, I used the pattern tools in Creo to generate the rest of the holes rather than drawing each one individually. With the wall being 40 mm wide and 30 mm high, and using that 7.5 mm offset from the edges, the pattern ended up with about 25 mm horizontal and 15 mm vertical spacing between the centers.


![A3](A_15.png)
Once I had that first wall hole set, I used a linear pattern to generate the rest of the attachment holes. It kept the four holes perfectly symmetrical and cut down on the number of separate dimensions I had to manage in the model.

I actually got a bit stuck here at first, wondering why the horizontal spacing was 25 mm while the vertical was only 15 mm. After double-checking the numbers, it clicked that the horizontal side spans 40 mm while the vertical is only 30 mm. Since I used a 7.5 mm offset from every edge, the center-to-center distances were bound to be different. It was a good reminder to actually look at the geometry instead of just blindly plugging numbers into Creo.


### Design features on the motor mount to minimize deflection.

![A3](A_17.png)

I ended up making one final adjusment to my part. To keep the mount stable without making the whole thing bulky, I decided to add triangular gussets between the motor-support and wall-support plates. By reinforcing the fixed corner where the bending moment is strongest, these gussets really stiffen up the assembly. It’s a great way to cut down on the deflection for Feature 1 without needing to increase the thickness of the entire mount.

## CAD FILE DOWNLOAD

[Download Motor Mount Creo CAD File (.zip)](CAD_FILE.zip)



