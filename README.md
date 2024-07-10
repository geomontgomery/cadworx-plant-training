# 1. CADWorx® Plant Training
<p align="center">
  <img src="bin/images/2b94ba08-bb0e-49fe-977f-6727fdb592cc.png" alt="chrome_rO5TB10M4C">
</p>

- [1. CADWorx® Plant Training](#1-cadworx-plant-training)
  - [1.1. About](#11-about)
  - [1.2. Before you Begin](#12-before-you-begin)
    - [1.2.1. Introduction](#121-introduction)
      - [1.2.1.1. Products](#1211-products)
  - [1.3. Session 1: Fundamental Skills](#13-session-1-fundamental-skills)
    - [1.3.1. Getting Started with CADWorx® (est 2 hours)](#131-getting-started-with-cadworx-est-2-hours)
      - [1.3.1.1. In this section](#1311-in-this-section)
      - [1.3.1.2. Launching and setup](#1312-launching-and-setup)
      - [1.3.1.3. Connecting to a Config File](#1313-connecting-to-a-config-file)
      - [1.3.1.4. Connecting to a Project File](#1314-connecting-to-a-project-file)
      - [1.3.1.5. Creating an initial route: Working with the primary functions of CADWorx](#1315-creating-an-initial-route-working-with-the-primary-functions-of-cadworx)
    - [1.3.2. Auto-Routing Options Review](#132-auto-routing-options-review)
    - [1.3.3. Palette Review](#133-palette-review)
  - [1.4. Hands-On Practice](#14-hands-on-practice)
    - [1.4.1. Construct Civil/Structural Foundation](#141-construct-civilstructural-foundation)
      - [1.4.1.1. Create the steel frame and foundation.](#1411-create-the-steel-frame-and-foundation)
    - [1.4.2. Hands-On Practice (1 hour)](#142-hands-on-practice-1-hour)
    - [1.4.3. Review and Wrap-Up (30 minutes)](#143-review-and-wrap-up-30-minutes)
  - [1.5. Session 2: Advanced Features and Practical Applications](#15-session-2-advanced-features-and-practical-applications)
    - [1.5.1. Recap and Introduction to Advanced Features (30 minutes)](#151-recap-and-introduction-to-advanced-features-30-minutes)
    - [1.5.2. Advanced Features (2 hours)](#152-advanced-features-2-hours)
    - [1.5.3. Hands-On Practice (1 hour)](#153-hands-on-practice-1-hour)
    - [1.5.4. Practical Applications (2 hours)](#154-practical-applications-2-hours)
    - [1.5.5. Hands-On Practice (1 hour)](#155-hands-on-practice-1-hour)
    - [1.5.6. Review and Wrap-Up (1 hour)](#156-review-and-wrap-up-1-hour)
- [2. Addendum](#2-addendum)
  - [2.1. About Me](#21-about-me)

## 1.1. About
This document outlines a two-day training course for CADWorx® Plant Professional by Hexagon®, a 3D plant design and modeling software that installs on top of AutoCAD® as an extension.  
The training is broken into two sections and emphasizes quickly learning and applying skills in piping design for new users. It's meant for new CADWorx® Plant end users who are primarly creating Orthographic and Isometric deliverables.  
It assumes the user has a basic understanding of AutoCAD®, and is familiar with the AutoCAD® command language.

## 1.2. Before you Begin
- Install AutoCAD® Plant 3D
- Install CADWorx® Plant
- Ensure both applications are licensed (CADWorx shortcut launches with no errors)
- Download the training.zip to your desktop and unzip.
### 1.2.1. Introduction
- Welcome and Introductions: Brief introduction of the trainer and participants
- Overview of CADWorx®: Purpose and benefits of the application
#### 1.2.1.1. Products
- CADWorx® Product Suite:
  - CADWorx® Plant: 3D piping for plant design and modeling software
  - CADWorx® Equipment: Specialized tool for equipment modeling and design
  - CADWorx® Structure: Structural steel and concrete modeling software
  - CADWorx® P&ID: Intelligent process and instrumentation diagramming tool
- ECE Design Plugins:
  - BUBBLEWorx: Tool for creating and managing bubble annotations in drawings
  - VIEWWorx: Utility for managing and customizing view settings in CADWorx®
  - ISOWorx: Solution for generating and managing isometric drawings
  - ANNOWorx: Tool for creating and managing annotations in CADWorx® models
  - MTOWorx: Material takeoff tool for generating accurate material lists

- Objectives of the Training: What the users will learn and achieve by the end of the training
## 1.3. Session 1: Fundamental Skills

### 1.3.1. Getting Started with CADWorx® (est 2 hours)
#### 1.3.1.1. In this section
- How to connect to a CADWorx Config file (.cfg) and a CADWorx Project File, (.prj)
- How to use Autorouting in CADWorx
- How to use the Specification View Palette
- How to use the Component List
#### 1.3.1.2. Launching and setup

  > _Note: before launching, consider right clicking the icon, going to properties, and setting /nologo on the shortcut to remove the AutoCAD startup logo._
  1. Download the training.zip to your desktop and unzip.
  2. Click the CADWorx® Plant icon on the desktop  
![CADWorx Plant Icon](bin/images/explorer_X4U6jG0SIt.png)  
     a. Optional: If it doesn't launch, you may run the setup profile utility:  
     ![Setup Profile Utility](bin/images/CADWorx_Setup_Profile_2ptfUritzk.png)  
     b. Optional: you might need to run the CADWorx64Wrapper batch file **(as an administrator)**:  
     ![Batch File Error](bin/images/acad_dvURfRMgI1.png)  
  > _Note: Did CADWorx launch successfully? Try running the CADWORXABOUT command in the command line to verify._
  3. Save a new drawing titled "start.dwg" in your ./training folder.
#### 1.3.1.3. Connecting to a Config File

  4. In AutoCAD, type in SETUP to select the config file. (*.cfg)  
  > _Note: Save your changes, but do not close the dialog._
     ![Configuration File](bin/images/acad_rCY8IHgiX0.gif)  
  5. In the setup dialog, go to Configuration Settings > "SpecificationDirectory". Select the "..." dialog and navigate to the ./training folder. Save Changes and close.  
> _Note: This sets the location where your *.prj files are stored for your project. Your company may have specific locations (or network locations) where *prj files are stored._

#### 1.3.1.4. Connecting to a Project File

  6. Open your spec view palette  
     ![Project File](bin/images/acad_kBWrdpfTIY.png)  
  7. Select your PRJ file and click open.  Then choose your specification (use a carbon steel class 150 for now)
     ![Selecting prj, spec, size](bin/images/acad_bnT2uXMhKP.gif)  

#### 1.3.1.5. Creating an initial route: Working with the primary functions of CADWorx

Let's get some piping components into the drawing, to get us started.

  8. Create an initial route:
  > _Note: Commands after "PIPW" are all ran **inside** that command_.

```
Z A
PIPW enter 0,0,0 enter
move east, 24  
choose 90 LR  
move north, 48  
move east, 24  
pick gate valve  
pick RF flange  
pick standard gasket  
left click on the right side of the route  
enter to end the command  
```
  ![Visual and Selection Preferences](bin/images/acad_zv1hWtiYAS.gif)

  9.  Edit the visual mode:
  > _Note: These are general visual settings for working in CADWorx® Plant.  They are not necessary but usually preferred._  

```
ISOLINES 0  
DISPSILH 1  
REGEN  

```

  10.  Hold down your left shift key and your middle mouse button to rotate the screen. Position to where you can see the 'starting' tie point in your route in an iso view.
  11.  Add elevation to the route:

```
Left click the design grip (+) on the open end of your route to continue autorouting.
west 24
P (to change plane to Z axis)
elevation 48
west 48
L (for component list)
Pick Blind Flange, and standard gasket.
```
![CADWorx Plant Training](bin/images/acad_xUeIhnwYIx.gif)

  12.  Add inline components
```
search for "check" in your spec view palette. select it.
Use S or E to change the flow of the check
Left click near the east end of the flanged gate connection, and click to add inline.
```
![CADWorx Plant Training](bin/images/acad_ENjKaFHYtN.gif)

  12.  Add tee components
```
select your pipe route near the origin and click the inline design grip (+)
type "mid" while placing tee, to select center of pipe.
south x.x
east x.x (near the middle of the east most route)
type "PER" and select the pipe route to connect to.
choose "TEE" from the dialog
```
![CADWorx Plant Training](bin/images/acad_BVUxsNzAYW.gif)

  12.  Add reducing components
```
c:CHANGESIZE Manual.
Select all components on the "bypass" you just routed, minus the the tees.
Choose 4" for the reduction size.
On the East connection, choose a reducing component (CONC reducer)
On the West connection, choose to change current component.
```
![CADWorx Plant Training](bin/images/acad_fUPkIPNzM8.gif)

  13.  Add inline olets
```
In your specview palette, change Main 4", Reduction 1".
Check your specview pallete settings > threaded on.
search or find "THRD-O-LET" in your specview pallete and select.
while placing the olet, type in NEA for a "near" snap.
click on the bypass parallel to the pipe route.
while placing along length of pipe, use "P" to select the east end, 2" away from weld.
place olet on the top pipe quadrant
```
![CADWorx Plant Training](bin/images/acad_4xuGtCaonJ.gif)

  13.  Route off olet
```
In your specview palette, change Main 4", Reduction 1".
Check your specview pallete settings > threaded on.
search or find "THRD-O-LET" in your specview pallete and select.
while placing the olet, type in NEA for a "near" snap.
click on the bypass parallel to the pipe route.
while placing along length of pipe, use "P" to select the east end, 2" away from weld.
place olet on the top pipe quadrant
```
![CADWorx Plant Training](bin/images/acad_4xuGtCaonJ.gif)

### 1.3.2. Auto-Routing Options Review
In this section we routed some components using various tools in the autoroute command. Let's take a closer look at the various commands available.

While Autorouting from NO start point, or the END of an open component, here are the various commands available:

<p align="left">
  <img src="bin/images/acad_jOVFKu2DRt.png" alt="CADWorx Plant Training">
</p>

| Command         | Description |
|-----------------|-------------|
| component <span style="color:orange">**L**</span>ist  |open component list, parts that can be routed with your current spec, fitting type, and nominal size.             |
| <span style="color:orange">**S**</span>lope           |slope the current route             |
| s<span style="color:orange">**K**</span>ew            |skew the current route by * degrees             |
| <span style="color:orange">**E**</span>levation       |elevate the current route            |
| <span style="color:orange">**P**</span>lane           |change the XY plane to XZ or ZY             |
| <span style="color:orange">**R**</span>eference       |change position based on other objects             |
| <span style="color:orange">**F**</span>itting Mode    |swap to socket, threaded, welded mode             |
| el<span style="color:orange">**B**</span>ow type      |change to LR, SR, miter el on autorout             |
| <span style="color:orange">**U**</span>ndo            |undo last step             |
| <span style="color:orange">**C**</span>onnect         |auto connect to a selected point             |
| <span style="color:orange">**T**</span>oggle Length   |measure length from elbow weld or corner             |
| <span style="color:orange">**A**</span>lignment       |align route to a pipe quadrant         |

While Autorouting from inline a pipe component, here are the various commands available:

<p align="left">
  <img src="bin/images/acad_TNnRONzZG6.png" alt="CADWorx Plant Training">
</p>

| Command         | Description |
|-----------------|-------------|
| component <span style="color:orange">**L**</span>ist            |open component list, for inline parts that can be routed with your current spec, fitting type, and nominal size.             |
| poin<span style="color:orange">**T**</span> distance            |pick a point to measure distance from             |
| <span style="color:orange">**C**</span>omponent distance        |pick a component to measure distance from             |
| <span style="color:orange">**P**</span>ipe end point distance   |toggle pipe end point measuring from            |
| insertion <span style="color:orange">**J**</span>ustification   |select part on your component to measure distance from             |

<center><span style="color:orange; font-size: 2em;">**Knowledge Check!**</span></center>


### 1.3.3. Palette Review

**Spec View Palette**

<p align="center">
  <img src="bin/images/ShareX_zPE60QYb5I.png" alt="CADWorx Plant Training">
</p>

> _Note: Many components can be dropped from the command line using their CADWorx command in CEDIT_

| Number | |
|--------|---|
| 1      |Spec View Settings (14,15,16)|
| 2      |Open Spec Editor   |
| 3      |Line Number Setup   |
| <span style="color:orange">**4**</span>      |c:C2A (Set size, spec, line num)    |
| <span style="color:orange">**5**</span>      |Current prj file   |
| <span style="color:orange">**6**</span>      |Current Main size   |
| <span style="color:orange">**7**</span>      |Current Reduction size   |
| <span style="color:orange">**8**</span>      |Current Specification   |
| <span style="color:orange">**9**</span>      |Current Line Number   |
| 10     |Search line numbers   |
| 11     |Search components   |
| 12     |Current components based on main/reduction and spec   |
| 13     |Custom data fields in PRJ file   |
| 14     |Color Options, how the component list (12) is colored   |
| 15     |Display Options, how the component list (12) is listed   |
| <span style="color:orange">**16**</span>     |Component Options, which components are shown based on type   |

**Line View Palette**

<p align="center">
  <img src="bin/images/ApplicationFrameHost_l9PNBvEAzF.png" alt="CADWorx Plant Training">
</p>

> _Note: Most of these settings can be controlled via the LINEISOLATE command._    
> _Consider editing your pgp file for quick access to LINEISOLATE_

| Number | |
|--------|---|
| 1      |Line view settings   |
| **2**      |Select component to isolate   |
| 3      |Select rows to isolate   |
| **4**      |Show All   |
| **5**      |Refresh line view list    |
| 6      |Full or Partial Isolation   |
| 7      |Line view list accordion panel   |
| 8      |Search filter Line view list   |
| 9      |List of line numbers and properties   |
| 10     |Advanced Search   |



**Clash Management Palette**
<p align="center">
  <img src="bin/images/ShareX_fpgZ0BOJK9.png" alt="Clash Management Palette">
</p>


| Number | |
|--------|---|
| 1      |Toggle clash detection   |
| 2      |Show or hide clashes   |
| 3      |Soft Clash Volume list   |
| 4      |Refresh, delete, zoom, or create new soft clash bodies   |
| 5      |Refresh hard clashes   |
| 6      |Zoom to selected clash   |

 _Note: A soft clash volume is typically an empty volume that is reserved for operational use._


**Discontinuity View Palette**

<p align="center">
  <img src="bin/images/acad_l2NNhPLB5J.png" alt="Discontinuity View Palette">
</p>

**Insulation Palette**

<p align="center">
  <img src="bin/images/acad_PovZKGyEe4.png" alt="Generated Image">
</p>

**Pipe Support Modeler**

<p align="center">
  <img src="bin/images/acad_kNBu2VGiYG.png" alt="Generated Image">
</p>


## 1.4. Hands-On Practice


<p align="center">
  <img src="bin\images\SumatraPDF_vv5jLDC2zS.png" alt="CADWorx Plant Training">
</p>

Guided excersise to construct a small skid piping model for a fictional project.

 - 2 pumps
 - Horizontal vessel
 - Vertical Vessel
 - ~6 pipe routes

### 1.4.1. Construct Civil/Structural Foundation

Here's what we'll do in this section

- Make a steel frame out of line segments, using SFRAME
- Create W-shape columns and Beams on the frame
- Create a Foundation with Piers, attached to the columns.
- Create secondary concrete pads for pumps.

#### 1.4.1.1. Create the steel frame and foundation.
1. Open CADWorx Structure.
2. Save a new drawing in training\e_projects\S1.dwg
3. c:SFRAME, using the guidelines below.

<p align="center">
  <img src="bin/images/acad_KKaRbqr7PW.png" alt="Generated Image">
</p>

4. Create the Columns and Beams per the following:

**Placing Columns**
```
Open shapes dialog, choose wide flange
Select Member: 10x26
Select Angle: 90
Select middle center cardinal point
Select Group: Columns
Select Place By: "Select Lines", and click Ok.
Pick all vertical lines to place beams.
```
> _Note: The orientation of the image of the beam is relative to true north._

<p align="center">
  <img src="bin/images/acad_PqfAUU5P9O.gif" alt="Generated Image">
</p>


**Placing Beams**
```
Open shapes dialog, choose wide flange
Select Member: 8x18
Select Angle: 0
Select **TOP** center cardinal point
Select Group: Beams
Select Place By: "Select Lines", and click Ok.
Pick all horizontal lines to place beams.
```

<p align="center">
  <img src="bin/images/acad_g5UUoqMO0g.gif" alt="Generated Image">
</p>


> _Note: If you need to edit the section size or other properties, you can edit multiple steel shapes at once by selecting multiple, then double clicking one of the selected._

5. Join the Columns

<p align="left">
  <img src="bin/images/acad_M5eQQGAG2y.png" alt="Generated Image">
</p>


6. Cope the Beams to the Columns with a welded cope.

<p align="left">
  <img src="bin/images/acad_iOXyRaw1el.png" alt="Generated Image">
</p>

Steps 5 and 6 below.

<p align="center">
  <img src="bin/images/acad_hEZVG7PoMk.gif" alt="Generated Image">
</p>


### 1.4.2. Hands-On Practice (1 hour)
- Guided Exercises: Tasks to practice using the core features
- Q&A Session: Address questions related to core features

### 1.4.3. Review and Wrap-Up (30 minutes)
- Recap of the Day: Summary of what was covered
- Q&A Session: Final questions for the day
- Preview of Day 2: What to expect in the next session

## 1.5. Session 2: Advanced Features and Practical Applications

### 1.5.1. Recap and Introduction to Advanced Features (30 minutes)
- Review of Day 1: Quick recap of core competencies
- Introduction to Advanced Features: Overview of what will be covered

### 1.5.2. Advanced Features (2 hours)
- Advanced Feature 1: Detailed explanation and demonstration
- Advanced Feature 2: Detailed explanation and demonstration
- Advanced Feature 3: Detailed explanation and demonstration

### 1.5.3. Hands-On Practice (1 hour)
- Guided Exercises: Tasks to practice using advanced features
- Q&A Session: Address questions related to advanced features

### 1.5.4. Practical Applications (2 hours)
- Real-World Scenarios: Applying CADWorx® to practical, real-world scenarios relevant to the users
- Case Studies: Examples and case studies of successful CADWorx® usage

### 1.5.5. Hands-On Practice (1 hour)
- Guided Exercises: Tasks based on real-world scenarios and case studies
- Q&A Session: Address questions related to practical applications

### 1.5.6. Review and Wrap-Up (1 hour)
- Recap of the Day: Summary of what was covered
- Q&A Session: Final questions for the day
- Next Steps: Resources for further learning and support
- Feedback Session: Collect feedback from the users about the training

# 2. Addendum

## 2.1. About Me

This training course is led by George Montgomery, M.E., a CAD Administration Consultant and Leica HDS Technical Sales and Support specialist. With extensive experience in both Leica and CAD systems, George brings a wealth of knowledge to this training:

- Expertise in Leica software and hardware sales and support
- Experience providing on-site training for Leica HDS and AutoCAD Plant 3D
- Proficiency in CAD administration, training, and support
- Background in generating project-specific templates and providing consulting feedback on 3D plant specifications

George's diverse skill set in both Leica and CAD systems ensures a comprehensive and practical approach to this CADWorx® Plant training course.
