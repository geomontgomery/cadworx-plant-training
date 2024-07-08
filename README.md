# 1. CADWorx® Plant Training
<p align="center">
  <img src="bin\images\2b94ba08-bb0e-49fe-977f-6727fdb592cc.png" alt="chrome_rO5TB10M4C">
</p>

- [1. CADWorx® Plant Training](#1-cadworx-plant-training)
  - [1.1. About](#11-about)
  - [1.2. Session 1: Core Competency](#12-session-1-core-competency)
    - [1.2.1. Introduction (45 minutes)](#121-introduction-45-minutes)
      - [1.2.1.1. Products](#1211-products)
    - [1.2.2. Getting Started with CADWorx® (2 hours)](#122-getting-started-with-cadworx-2-hours)
      - [In this section](#in-this-section)
      - [Launching and setup](#launching-and-setup)
      - [Connecting to a Config File](#connecting-to-a-config-file)
      - [Connecting to a Project File](#connecting-to-a-project-file)
      - [Navigating the Interface: Overview of the user interface, menus, and key functions](#navigating-the-interface-overview-of-the-user-interface-menus-and-key-functions)
    - [1.2.3. Hands-On Practice (1 hour)](#123-hands-on-practice-1-hour)
    - [1.2.4. Core Features (2 hours)](#124-core-features-2-hours)
    - [1.2.5. Hands-On Practice (1 hour)](#125-hands-on-practice-1-hour)
    - [1.2.6. Review and Wrap-Up (30 minutes)](#126-review-and-wrap-up-30-minutes)
  - [1.3. Session 2: Advanced Features and Practical Applications](#13-session-2-advanced-features-and-practical-applications)
    - [1.3.1. Recap and Introduction to Advanced Features (30 minutes)](#131-recap-and-introduction-to-advanced-features-30-minutes)
    - [1.3.2. Advanced Features (2 hours)](#132-advanced-features-2-hours)
    - [1.3.3. Hands-On Practice (1 hour)](#133-hands-on-practice-1-hour)
    - [1.3.4. Practical Applications (2 hours)](#134-practical-applications-2-hours)
    - [1.3.5. Hands-On Practice (1 hour)](#135-hands-on-practice-1-hour)
    - [1.3.6. Review and Wrap-Up (1 hour)](#136-review-and-wrap-up-1-hour)
- [2. Addendum](#2-addendum)
  - [2.1. About Me](#21-about-me)

## 1.1. About
This document outlines a two-day training course for CADWorx® Plant Professional by Hexagon®, a 3D plant design and modeling software that installs on top of AutoCAD® as an extension.  
The training is broken into two sections and emphasizes quickly learning and applying skills in piping design for new users. It's meant for new CADWorx® Plant end users who are primarly creating Orthographic and Isometric deliverables.  
It assumes the user has a basic understanding of AutoCAD®, and is familiar with the AutoCAD® command language.

## 1.2. Session 1: Core Competency
### 1.2.1. Introduction (45 minutes)
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

### 1.2.2. Getting Started with CADWorx® (2 hours)
#### In this section
How to connect to a CADWorx Config file (.cfg) and a CADWorx Project File, (.prj). This enables most of the following functionality while using CADWorx.
#### Launching and setup

  > _Note: before launching, consider right clicking the icon, going to properties, and setting /nologo on the shortcut to remove the AutoCAD startup logo._
  1. Download the training.zip to your desktop and unzip.
  2. Click the CADWorx® Plant icon on the desktop  
![CADWorx Plant Icon](bin\images\explorer_X4U6jG0SIt.png)  
     a. Optional: If it doesn't launch, you may run the setup profile utility:  
     ![Setup Profile Utility](bin\images\CADWorx_Setup_Profile_2ptfUritzk.png)  
     b. Optional: you might need to run the CADWorx64Wrapper batch file **(as an administrator)**:  
     ![Batch File Error](bin\images\acad_dvURfRMgI1.png)  
  > _Note: Did CADWorx launch successfully? Try running the CADWORXABOUT command in the command line to verify._
  3. Save a new drawing titled "start.dwg" in your ./training folder.
#### Connecting to a Config File

  4. In AutoCAD, type in SETUP to select the config file. (*.cfg)  
  > _Note: Save your changes, but do not close the dialog._
     ![Configuration File](bin\images\acad_rCY8IHgiX0.gif)  
  5. In the setup dialog, go to Configuration Settings > "SpecificationDirectory". Select the "..." dialog and navigate to the ./training folder. Save Changes and close.
#### Connecting to a Project File

  6. Open your spec view palette  
     ![Project File](bin\images\acad_kBWrdpfTIY.png)  
  7. Select your PRJ file and click open.  Then choose your specification (use a carbon steel class 150 for now)
     ![Selecting prj, spec, size](bin\images\acad_bnT2uXMhKP.gif)  

#### Navigating the Interface: Overview of the user interface, menus, and key functions
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
  ![Visual and Selection Preferences](bin\images\acad_zv1hWtiYAS.gif)

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
![CADWorx Plant Training](bin\images\acad_xUeIhnwYIx.gif)

  12.  Add inline components
```
search for "check" in your spec view palette. select it.
Use S or E to change the flow of the check
Left click near the east end of the flanged gate connection, and click to add inline.
```
![CADWorx Plant Training](bin\images\acad_ENjKaFHYtN.gif)

  12.  Add tee components
```
select your pipe route near the origin and click the inline design grip (+)
type "mid" while placing tee, to select center of pipe.
south x.x
east x.x (near the middle of the east most route)
type "PER" and select the pipe route to connect to.
choose "TEE" from the dialog
```
![CADWorx Plant Training](bin\images\acad_BVUxsNzAYW.gif)

  12.  Add reducing components
```
c:CHANGESIZE Manual.
Select all components on the "bypass" you just routed, minus the the tees.
Choose 4" for the reduction size.
On the East connection, choose a reducing component (CONC reducer)
On the West connection, choose to change current component.
```
![CADWorx Plant Training](bin\images\acad_fUPkIPNzM8.gif)

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
![CADWorx Plant Training](bin\images\acad_4xuGtCaonJ.gif)



### 1.2.3. Hands-On Practice (1 hour)
- Guided Exercises: Simple tasks to practice the basic operations
- Q&A Session: Address any initial questions or concerns

### 1.2.4. Core Features (2 hours)
- Feature 1: Detailed explanation and demonstration of a core feature
- Feature 2: Detailed explanation and demonstration of another core feature
- Feature 3: Detailed explanation and demonstration of an additional core feature

### 1.2.5. Hands-On Practice (1 hour)
- Guided Exercises: Tasks to practice using the core features
- Q&A Session: Address questions related to core features

### 1.2.6. Review and Wrap-Up (30 minutes)
- Recap of the Day: Summary of what was covered
- Q&A Session: Final questions for the day
- Preview of Day 2: What to expect in the next session

## 1.3. Session 2: Advanced Features and Practical Applications

### 1.3.1. Recap and Introduction to Advanced Features (30 minutes)
- Review of Day 1: Quick recap of core competencies
- Introduction to Advanced Features: Overview of what will be covered

### 1.3.2. Advanced Features (2 hours)
- Advanced Feature 1: Detailed explanation and demonstration
- Advanced Feature 2: Detailed explanation and demonstration
- Advanced Feature 3: Detailed explanation and demonstration

### 1.3.3. Hands-On Practice (1 hour)
- Guided Exercises: Tasks to practice using advanced features
- Q&A Session: Address questions related to advanced features

### 1.3.4. Practical Applications (2 hours)
- Real-World Scenarios: Applying CADWorx® to practical, real-world scenarios relevant to the users
- Case Studies: Examples and case studies of successful CADWorx® usage

### 1.3.5. Hands-On Practice (1 hour)
- Guided Exercises: Tasks based on real-world scenarios and case studies
- Q&A Session: Address questions related to practical applications

### 1.3.6. Review and Wrap-Up (1 hour)
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
