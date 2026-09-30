# MechaMinds-WRO 2026 Future Engineers
# WRO Future Engineers - Engineering Documentation
## Team Members
- **Barbara Lukić**
- **Nadia Kravčuk**
- **Ivano Koren**

<img src="media/team/team.jpeg" width="500" >

## Table of Contents

- [1. Project Overview](#1-project-overview)
- [2. Team](#2-team)
- [3. Vehicle Overview](#3-vehicle-overview)

- [4. Development History](#4-development-history)
  - [4.1 Version 1](#41-version-1)
  - [4.2 Version 2](#42-version-2)
  - [4.3 Version 3](#43-version-3)
  - [4.4 Version 4](#44-version-4)
  - [4.5 Current Robot](#45-current-robot)
 
- [5. Mobility & Mechanical Design](#5-mobility--mechanical-design)
  - [5.1 Chassis](#51-chassis)
   - [5.2 Drive System](#52-drive-system)
  - [5.3 Steering System](#53-steering-system)
  - [5.4 Dimensions and Weight](#54-dimensions-and-weight)
  
- [6. Power & Sensor Architecture](#6-power--sensor-architecture)
  - [6.1 Motors](#61-motors)
  - [6.2 Sensors](#62-sensors)
  - [6.3 Sensor Placement](#63-sensor-placement)
  - [6.4 Wiring Diagram](#64-wiring-diagram)
  - [6.5 Power](#65-power)
  - [6.6 ON/OFF Button](#66-onoff-button)
  
- [7. Software Architecture](#7-software-architecture)
  - [7.1 Overview](#71-overview)
  - [7.2 Code](#72-code)
  - [7.3 Open Challenge Strategy](#73-open-challenge-strategy)
  - [7.4 Obstacle Challenge Strategy](#74-obstacle-challenge-strategy)
    
- [8. Engineering Decisions](#8-engineering-decisions)
  - [8.1 Constraints](#81-constraints)
  - [8.2 Major Problems and Solutions](#82-major-problems-and-solutions)

- [9. Testing & Results](#9-testing--results)
  - [9.1 Mechanical Tests](#91-mechanical-tests)
  - [9.2 Sensor Tests](#92-sensor-tests)

- [10. Components / Bill of Materials](#10-components--bill-of-materials)

- [11. Build & Reproduction Guide](#11-build--reproduction-guide)
  - [11.1 Parts](#111-parts)
  - [11.2 Assembly](#112-assembly)

- [12. Repository Structure](#12-repository-structure)
- [13. Engineering Journal](#13-engineering-journal)


## 1. Project Overview
Our project is an autonomous vehicle that can navigate the competition field, detect and avoid obstacles, follow the track and make real time decisions without human intervention.

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 2. Team
We are Croatia robotics team **MechaMinds** and our names are **Barbara Lukić**, **Ivano Koren** and **Nadia Kravčuk**. We come from high school Tin Ujević in Kutina. Our mentors name is Damir Petravić. Together we worked on design of the robot, programming and testing our robot.

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 3. Vehicle Overview
| Specification | Value |
|---|---|
| Length | 18 cm |
| Width | 17.5 cm |
| Height | 15.5 cm |
| Weight | 0.876 kg |
| Drive type | Rear-wheel drive |
| Steering type | Ackermann steering |     ---Servo-controlled front steering???
| Main controller | Raspberry Pi 5 Model (B Rev1.1) |
| Programming language | C++ |
| Main sensors | MRMS LIDAR 2 m (VL53L0CX), CAN Bus |
| Camera | Raspberry Pi Camera Module 3 |
| Power source | Turnigy 5S LiPo, 18.5 V, 5000 mAh |

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 4. Development history 
Our robot went through several major design changes during the development process.
### 4.1. Version 1 
**About the robot** 
  - Our first robot was a custom-build vehicle made using 3D-prined and hand-build parts. It had several distance
sensors that helped us test the robot.

**Main problem** 
  - The robot was not realible in making 3 laps so we decided to change the robot for better performance.

| Front | Rear |
|---|---|
| <img src="media/development/version_1/front.jpeg" width="200"> | <img src="media/development/version_1/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_1/left.jpeg" width="200"> | <img src="media/development/version_1/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_1/top.jpeg" width="200"> | <img src="media/development/version_1/bottom.jpeg" width="200"> |

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 4.2. Version 2
**About the robot**
- This robot was an upgraded version on the first one, it had a camera and several distance sensors.
  
**Main problem**
- All year we have been working on this robot, about two months before the competition we started having problems connecting the robot to Wi-Fi, it started crashing and we tried to find a solution before the competition but we did not succeed.

| Front | Rear |
|---|---|
| <img src="media/development/version_2/final/front.jpeg" width="200"> | <img src="media/development/version_2/final/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_2/final/left.jpeg" width="200"> | <img src="media/development/version_2/final/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_2/final/top.jpeg" width="200"> | <img src="media/development/version_2/final/bottom.jpeg" width="200"> |

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 4.3. Version 3
**About the robot**
- This robot that we had build out of LEGO, it represents a model of a Ford car.

**Main problem**
- Robot had a problem turning its wheels because of the design, so it could not compleate even one lap, beacuse of this we had to completaly redesign it.

| Front | Rear |
|---|---|
| <img src="media/development/version_3/front.jpeg" width="200"> | <img src="media/development/version_3/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_3/left.jpeg" width="200"> | <img src="media/development/version_3/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_3/ford1.jpeg" width="200"> | <img src="media/development/version_3/bottom.jpeg" width="200"> |

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 4.4. Version 4
**About the robot**
- This was our final robot that we went to the competition with, it was also build out of lego bricks, it worked with help of distance sensors.
  
**Main problem**
- Although we went to the competition with this robot it still had a few flaws. The LEGO sensors that we used to measure distance were not able to detect walls from sufficient distance so the robot couldn't compleate even one lap.

| Front | Rear |
|---|---|
| <img src="media/development/version_4/front.jpeg" width="200"> | <img src="media/development/version_4/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_4/left.jpeg" width="200"> | <img src="media/development/version_4/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_4/top.jpeg" width="200"> | <img src="media/development/version_4/bottom.jpeg" width="200"> |

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 4.5 Current Robot
The robot we are using for competition in Zagreb will be [4.2 Version 2](#42-version-2) 

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 5. Mobility & Mechanical Design
### 5.1 Chassis

#### Chassis Overview
Our current vehicle uses a four-wheel chassis designed for the WRO Future Engineers challenge. The chassis provides the mechanical base for the drive system, steering mechanism, sensors and processing hardware. The design was developed with stability, compact dimensions and reliable steering in mind.

#### Material and Construction
Our robot is completly made out of 3D-printed parts. The parts are explained in section 11.

#### Component Placement
The electronic components are arranged on several levels above the main chassis plate. The battery is positioned low inside the chassis, while the processing and control electronics are mounted above it. The camera is mounted at the front of the robot on a dedicated 3D-printed support. The distance sensors are positioned near the front of the vehicle so that they can detect the surrounding walls during navigation.

(gdje se nalaze no) **TU CE ICI SLIKA SVEGA**
- Main controller: on top of the robot
- Battery: inside the chassis
- Drive motor: in the back, underneath the chassis
- Steering servo: in the front, underneath the chasis
- Sensors: in the front, inside the chassis
- Camera: the front of the robot

#### Design Reasoning

The battery was positioned low in the chassis to keep the center of gravity as low as possible.
We placed sensors at the front and inside the chasis because we found that in these positions the results were much better.
The button used to turn the robot on, start it, and stop it was placed on top to make it easily accessible.
Camera was placed in the front of the robot so it could have good visibility of the field.

#### Chassis Improvements

During testing, the distance sensors were positioned on the upper part of the robot. In this position, the sensors were too high and could not reliably detect the wall directly in front of the vehicle. After identifying this issue, we redesigned the sensor position and moved the distance sensors lower on the chassis. This improved their field of view and allowed them to detect the wall more reliably. This change showed us how strongly sensor placement can affect the performance of the navigation system.


<img src="media/development/version_2/build/build-03.jpeg" width="250">  <img src="media/development/version_2/build/build-04.jpeg" width="250">

**Test result:**
| Sensor position | Successful wall detections |
|---|---:|
| Original higher position | 4/10 |
| Lowered position | 8/10 |
????????????

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 5.2 Drive System

**TU TREBA SLIKA OD DOLJE I ZADNJI KOTACI (POGON)**

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 5.3 Steering System

The vehicle uses a servo-controlled front steering mechanism. A steering servo mounted at the front of the chassis moves a mechanical linkage that connects the two front wheels. Instead of controlling the left and right wheels with separate motors, both front wheels are mechanically linked and change direction together. This provides car-like steering while the rear wheels make the robot move forward. The steering components are mounted directly to the 3D-printed chassis, which allowed us to adjust the geometry and mounting positions during development.

<p align="center">
  <img src="media/development/version_2/final/bottom.jpeg" width="500">
</p>

<p align="center">
  <em>Front steering mechanism and mechanical linkage.</em>
</p>

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 5.4 Dimensions and Weight

| Measurement | Value |
|---|---|
| Length | 180 mm |
| Width | 175 mm |
| Height | 155 mm |
| Weight | TODO g |
| Wheelbase | 100 mm |
| Front track width | 175 mm |
| Rear track width | 170 mm |
| Front wheel diameter | 60 mm |
| Rear wheel diameter | 65 mm |

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>


## 6. Power & Sensor Architecture
### 6.1 Motors

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 6.2 Sensors

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 6.3 Sensor Placement

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 6.4 Wiring Diagram

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 6.5 Power

#### Battery

Our robot is powered by a Turnigy 5.0 High Discharge LiPo battery. 
The battery was selected to provide sufficient voltage, capacity and 
current for the robot's motors and electronic components.

#### Specifications

| Parameter | Value |
|---|---|
| Battery type | LiPo (Lithium Polymer) |
| Configuration | 5S |
| Nominal voltage | 18.5 V |
| Capacity | 5000 mAh (5.0 Ah) |
| Discharge rating | 20–30C |
| Maximum theoretical discharge current | 150 A |
| Manufacturer | Turnigy |
| Model | Turnigy 5.0 |
| Main connector | High-current connector |
| Balance connector | 5S balance connector |

We chose this battery because our robot requires a power source capable of 
supplying high current to the motors while maintaining a stable voltage.

<img src="media/power/battery/battery1.jpeg" width="200"> <img src="media/power/battery/battery3.jpeg" width="200"> <img src="media/power/battery/battery4.jpeg" width="200">
#### Charger

The robot uses a B6 LiPro 80W Balance Charger to charge the LiPo battery. It supports 1–6 cell LiPo batteries and includes a balance function to keep the voltage of the individual cells equal during charging.

<img src="media/power/charger/charger1.jpeg" width="200">

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 6.6 ON/OFF Button
<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>
<p>This section explains the code structure and button controls for operating the robot.</p>

<h4 align="center">Code for Buttons</h4>

<p align="center">
  <img src="media/buttons/button1.jpeg" alt="Code for Buttons" width="80%" />
</p>

<p align="center">
  <img src="media/buttons/button2.jpeg" alt="Physical Buttons on Robot" width="50%" />
</p>

<h4>Button Functions</h4>

<p><strong>1. Button 1 (Pin 1) &ndash; Start / Stop:</strong> Launches <code>system_start()</code> or halts the robot with <code>full_stop()</code>.</p>

<p><strong>2. Button 2 (Pin 2) &ndash; Open Challenge:</strong> Selects and starts <code>open_challenge()</code>.</p>

<p><strong>3. Button 3 (Pin 3) &ndash; Obstacle Challenge:</strong> Selects and starts <code>prepreke_challenge()</code>.</p>

<p><strong>4. Button 4 (Pin 4) &ndash; Servo +2°:</strong> Manually increases the servo angle by 2 degrees.</p>

<p><strong>5. Button 5 (Pin 5) &ndash; Servo Reset:</strong> Resets the servo angle back to 0°.</p>

## 7. Software Architecture
### 7.1 Overview

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 7.2 Code
<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 7.3 Open Challenge Strategy

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 7.4 Obstacle Challenge Strategy

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>


## 8. Engineering Decisions
### 8.1 Constraints

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 8.2 Major Problems and Solutions
#### Connection Failure 

- During development, we experienced repeated problems with the Wi-Fi connection between the robot and the development computer. The connection was unstable and we could not work with the robot properly. To improve reliability, we tested a wired Ethernet connection using an RJ45 network cable. During our tests, this connection proved to be significantly more stable and reliable than Wi-Fi, so we decided to use the wired connection during development.

<img src="media/connection-solution/connection1.jpeg" width="200"> <img src="media/connection-solution/connection2.jpeg" width="200">
<img src="media/connection-solution/connection3.jpeg" width="200"> <img src="media/connection-solution/connection4.jpeg" width="200">

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 9. Testing & Results
### 9.1 Mechanical Tests

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 9.2 Sensor Tests
tu ide video s ytuba kad stavimo ruku on skrece

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>
  
## 10. Components / Bill of Materials

[View the Bill of Materials PDF](docs/bill-of-materials/bill-of-materials.pdf)

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 11. Build & Reproduction Guide
### 11.1 Parts
-**wheels**:

 <img src="media/wheels-making/wheels1.jpeg" width="200">  <img src="media/wheels-making/wheels2.jpeg" width="200">  <img src="media/wheels-making/wheels3.jpeg" width="200">


-**wheels**

<img src="media/wheels-making/wheels2.jpeg" width="200">  <img src="media/wheels-making/wheels3.jpeg" width="200">


<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

### 11.2 Assembly

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>


## 12. Repository Structure
This repository is organized into separate folders for documentation, hardware, software, media and testing. It makes it easier to locate files needed to understand and reproduce the robot.

```text
WRO/
├── README.md
│
├── backup photos/
│   └── lego - mechaminds
│
├── docs/
│   ├── archive/
│   ├── bill-of-materials/
│   ├── images/
│   ├── build-guide.md
│   ├── engineering-decisions.md
│   ├── mechanical-design.md
│   ├── power-and-sensor.md
│   ├── software-arhitecture.md
│   └── testing.md
│
├── hardware/
│
├── media/
│   ├── connection-solution/
│   ├── development/
│   │   ├── version_1/
│   │   ├── version_2/
│   │   │   ├── build/
│   │   │   └── final/
│   │   ├── version_3/
│   │   ├── version_4/
│   │   └── version_4.1/
│   │       ├── before-repair/
│   │       ├── final/
│   │       ├── repair-process/
│   │       └── testing/
│   │
│   ├── final-robot/
│   ├── team/
│   ├── team2
│   ├── team3
│   └── team4
│
├── obstacle challenge/
├── open challenge/
├── Other/
├── software/
└── tests/
```

**OVO JE PODLOZNO MJENJANU NECE OVAK NIS BIT SAM DA VIDIMO KAK TREBA IZGLEDAT**

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>

## 13. Engineering Journal

<p align="right">
  <a href="#table-of-contents">⬆ Back to Table of Contents</a>
</p>
