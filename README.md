# Force Plates Vertical Force Verification - CMAS standards QA Test in Visual3D 

### Overview
This pipeline script (.v3s) and Visual 3D report template (.rgt) is what we use in the Derby lab as a force plate test to meet item 2.10 of the CMAS standards (v15, 2021):

**_"System checks undertaken each day the system is used should include placing at least 25kg onto the force plate to check the accuracy of the vertical force measurement"_**

We have 4 force plates so rather than dragging calibrated weights from plate to plate we take an acquisition in which the user stands **still** on each plate for around 10 seconds. Output vertical force can then be verified from the subject's weight. Forces in the plane of the floor can also be checked to ensure they are close to zero.

Output report includes X,Y,Z components of force from each plate (converted to equivalent mass) and vertical force graph includes a horizontal line marking the user's mass for easy comparison. (Note, our lab uses a 'Y up' system, so we refer to Fy as the vertical force where other labs likely use Fz).

This is a quick, visual comparison but there is scope to output the force data from the c3d for closer inspection.

### Instructions

1. Load the .c3d file to the visual 3d workspace  (Example data file in the repository)
2. Load and run the pipeline script
3. Open the report template (although the pipeline script will open this anyway, if the filepath is specified)

### Requirements
Visual 3d (C-motion). Any version should work but we are currently running version 6.

### Other Notes
Our system will sometimes crash if we take an acquisition without any 3d data when it is expecting it so the subject will usually be holding a reflective marker in view of the cameras during the acquisition. (This is quicker and easier than going into the settings to deselect 3d data capture).

These instructions assume you already have a working knowledge of Visual 3D and will be able to modify the report template to suit your lab's force plate setup, but I'm happy to try and help out if you're experiencing problems doing so.

### Contact 
martin.kerr1@nhs.net

![image](https://user-images.githubusercontent.com/50867224/150538085-ad78ad72-f2fb-411e-9b3d-1c876c41a0cb.png)
