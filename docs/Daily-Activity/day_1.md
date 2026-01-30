**1. Activity of Day 1**

**Home**
## Student Introduction
**Name:** HITAYEZU Emile  
**Program:** Master’s in IoT Embedded Computing Systems (University of Rwanda)  
**Reg_number:** 218001312  
**Website Purpose:** Document my digital modeling and fabrication learning process using MkDocs Material.
# Digital Modeling

**Modeling Approach**

My modeling approach follows a structured workflow:

1. Understand the problem and define requirements

2. Sketch the idea with dimensions and constraints

3. Create a clean 3D model using features (extrude, cut, fillet, chamfer)

4. Validate the design for fabrication (tolerances, thickness, alignment)

5. Export fabrication-ready files (STL/DXF/STEP)

**Design Decisions (Justification)**

Key decisions I considered during modeling:

- **Dimensions:** chosen to match real measurements and assembly needs

- **Thickness:** selected based on material strength and machine capability

- **Holes and clearances:** included tolerances to ensure parts fit after fabrication

- **Simplicity:** minimized unnecessary features to reduce fabrication errors

- **Reproducibility:** designed parts that are easy to remake and measure

**Modeling Workflow (Step-by-step)**

### Step 1  Requirements
- Functional purpose of the object

- Size limits (based on machine working area)

- Strength and durability needs

- Assembly method (screws, press-fit, glue, clips)

**Step 2  Sketching**
- Created sketches with constraints (horizontal, vertical, equal, symmetry)
- Fully constrained sketches to reduce future errors

**Step 3  3D Features**
- Extruded main body

- Added holes/cutouts

- Applied fillets/chamfers where needed (strength + better finishing)

**Step 4 Exporting Files**
Exported the model into formats used for fabrication:

- **STL:** for 3D printing

- **DXF:** for laser cutting (if needed)

- **STEP:** for sharing/editing and keeping exact geometry

-------------------------------------------------------------------------------------
# Fabrication Logic

## Machines (Fabrication Options)
Depending on the design, the fabrication process can use:

- **3D Printer (FDM):** good for complex shapes and enclosures 

- **Laser Cutter:** best for 2D profiles (acrylic/MDF) and fast prototyping 

- **CNC Milling:** good for precise machining, but requires toolpath planning 


## Materials
Material selection depends on strength, availability, and finishing: 

- **PLA:** easy to print, good for prototypes (not good for high heat) 

- **PETG:** stronger and more flexible than PLA 

- **Acrylic/MDF:** common for laser cutting, good for flat parts 

## Fabrication Constraints (Important)
These constraints affected design decisions: 

- **Minimum wall thickness:** too thin may break or warp 

- **Tolerance:** parts shrink/expand; holes may print smaller than designed

- **Overhang limits (3D printing):** steep overhangs require supports 

- **Bed size / working area:** design must fit machine dimensions 

- **Kerf (laser cutting):** laser removes a small width; affects fit 

- **Tool diameter (CNC):** inside corners cannot be perfectly sharp 
 
## Fabrication Settings (Example Template)
Fill these based on your machine:
- Machine: ____________________ 

- Material: ____________________ 

- Layer height (3D print): ____________________

- Infill: ____________________ 

- Supports: Yes / No 

- Laser power/speed (if laser): ____________________ 

- CNC tool diameter (if CNC): ____________________ 

## Fabrication Plan (Process)
1. Export file (STL/DXF) 

2. Prepare in slicer/CAM (set parameters) 

3. Fabricate on machine 

4. Inspect dimensions and quality 

5. Record issues and decide improvements 

-------------------------------------------------------------------------------
# Prototyping & Iteration

## Why Prototyping Matters
Prototyping helps validate the design before final production. It reveals:
- sizing mistakes
- tolerance issues
- weak points
- assembly difficulties

## Prototype 1
### Test Goal
The purpose of Prototype 1 was to test:
- overall size
- part fit and alignment
- strength of thin areas
- assembly method

### Observed Problems (Failures)
Common issues that may occur:
- holes too tight or too loose
- warping (3D printing)
- weak joints due to thin walls
- dimensions slightly off due to shrinkage/kerf

### Improvements Made
Based on Prototype 1:
- Increased/decreased hole diameter by a small tolerance
- Increased wall thickness for strength
- Adjusted clearances for press-fit parts
- Simplified geometry to reduce supports/cutting errors


## Prototype 2 (Improved Version) 
### What Changed 
- Applied the improvements found in Prototype 1
- Re-tested fit, strength, and finishing

### Result
Prototype 2 performed better because:
- improved tolerances
- better structural strength
- easier assembly

## Final Outcome
The final design is considered complete when:
- it can be fabricated reliably
- the assembly works as planned
- dimensions match requirements
- documentation is clear enough for reproduction
