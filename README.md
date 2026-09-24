# MechaMinds-WRO 2026 Future Engineers
# WRO Future Engineers - Engineering Documentation
# Team Members
- **Nadia Kravčuk**-
- **Ivano Koren**-Ivano spearheaded the physical construction of the vehicle, optimizing the chassis layout, steering geometry, and weight distribution, while the team assisted in testing mechanical durability.
- **Barbara Lukić**

<img src="media/team/team.jpeg" width="500" height="500">

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
  - [4.6 Crash / Failure Analysis and Redesign](#46-crash--failure-analysis-and-redesign)
 
- [5. Mobility & Mechanical Design](#5-mobility--mechanical-design)
  - [5.1 Chassis](#51-chassis)
   - [5.2 Drive System](#52-drive-system)
  - [5.3 Steering System](#53-steering-system)
  - [5.4 Dimensions and Weight](#54-dimensions-and-weight)
  - [5.5 Torque / Speed Reasoning](#55-torque--speed-reasoning)
  - [5.6 Mechanical Testing and Iterations](#56-mechanical-testing-and-iterations)

- [6. Power & Sensor Architecture](#6-power--sensor-architecture)
  - [6.1 Controller](#61-controller)
  - [6.2 Motors](#62-motors)
  - [6.3 Sensors](#63-sensors)
  - [6.4 Sensor Placement](#64-sensor-placement)
  - [6.5 Wiring Diagram](#65-wiring-diagram)
  - [6.6 Power Architecture](#66-power-architecture)
  - [6.7 Sensor Calibration and Testing](#67-sensor-calibration-and-testing)

- [7. Software Architecture](#7-software-architecture)
  - [7.1 Overview](#71-overview)
  - [7.2 Program Structure](#72-program-structure)
  - [7.3 State Machine / Flowchart](#73-state-machine--flowchart)
  - [7.4 Open Challenge Strategy](#74-open-challenge-strategy)
  - [7.5 Obstacle Challenge Strategy](#75-obstacle-challenge-strategy)
  - [7.6 Control Algorithms](#76-control-algorithms)
  - [7.7 Edge Cases and Failure Handling](#77-edge-cases-and-failure-handling)

- [8. Engineering Decisions](#8-engineering-decisions)
  - [8.1 Constraints](#81-constraints)
  - [8.2 Design Trade-offs](#82-design-trade-offs)
  - [8.3 Major Problems and Solutions](#83-major-problems-and-solutions)
  - [8.4 Why We Chose X Instead of Y](#84-why-we-chose-x-instead-of-y)

- [9. Testing & Results](#9-testing--results)
  - [9.1 Mechanical Tests](#91-mechanical-tests)
  - [9.2 Sensor Tests](#92-sensor-tests)
  - [9.3 Open Challenge Tests](#93-open-challenge-tests)
  - [9.4 Obstacle Challenge Tests](#94-obstacle-challenge-tests)
  - [9.5 Reliability Results](#95-reliability-results)

- [10. Components / Bill of Materials](#10-components--bill-of-materials)

- [11. Build & Reproduction Guide](#11-build--reproduction-guide)
  - [11.1 Parts](#111-parts)
  - [11.2 Assembly](#112-assembly)
  - [11.3 Wiring](#113-wiring)
  - [11.4 Software Installation](#114-software-installation)
  - [11.5 Uploading / Running the Code](#115-uploading--running-the-code)

- [12. Repository Structure](#12-repository-structure)
- [13. Version History](#13-version-history)
- [14. Engineering Journal](#14-engineering-journal)
- [15. Authors / Team](#15-authors--team)

## 1. Project Overview
## 2.Team
## 3.Vehicle Overview
| Specification | Value |
|---|---|
| Length | _ cm |
| Width | _ cm |
| Height | _ cm |
| Weight | _ |
| Drive type | Rear-wheel drive |
| Steering type | Ackermann steering |
| Main controller | Rasberry Pi 5 Model (B Rev1.1) |
| Programming language | C++ |
| Main sensors | ___ |
| Camera | ______ |
| Power source | ______ |

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

### 4.2. Version 2
- about the robot: this robot was an upgraded version on the first one, it had a camera and several distance sensors 
- problem: all year we have been working on this robot, about two months before the competition we started having problems connecting the robot to Wi-Fi, it started crashing and we tried to find a solution before the competition but we did not succeed

| Front | Rear |
|---|---|
| <img src="media/development/version_2/final/front.jpeg" width="200"> | <img src="media/development/version_2/final/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_2/final/left.jpeg" width="200"> | <img src="media/development/version_2/final/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_2/final/top.jpeg" width="200"> | <img src="media/development/version_2/final/bottom.jpeg" width="200"> |
### 4.3. Version 3
- about the robot: this robot that we had build out of LEGO, it represents a model of a ford car 
- problem: robot had a problem turning its wheels beacuse of the design, so it could not compleate even one lap, beacuse of this, we had to completaly redesing it

| Front | Rear |
|---|---|
| <img src="media/development/version_3/front.jpeg" width="200"> | <img src="media/development/version_3/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_3/left.jpeg" width="200"> | <img src="media/development/version_3/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_3/ford1.jpeg" width="200"> | <img src="media/development/version_3/bottom.jpeg" width="200"> |

### 4.4. Version 4
- about the robot: this was our final robot that we went to the competition with, it was also build out of lego bricks, it worked with help of distance sensors 
- problem: ????

| Front | Rear |
|---|---|
| <img src="media/development/version_4/front.jpeg" width="200"> | <img src="media/development/version_4/rear.jpeg" width="200"> |

| Left | Right |
|---|---|
| <img src="media/development/version_4/left.jpeg" width="200"> | <img src="media/development/version_4/right.jpeg" width="200"> |

| Top | Bottom |
|---|---|
| <img src="media/development/version_4/top.jpeg" width="200"> | <img src="media/development/version_4/bottom.jpeg" width="200"> |

### 4.5 Current Robot
### 4.6 Crash / Failure Analysis and Redesign

## 5. Mobility & Mechanical Design
### 5.1 Chassis

#### Chassis Overview
Our current vehicle uses a four-wheel chassis designed for the WRO Future Engineers challenge. The chassis provides the mechanical base for the drive system, steering mechanism, sensors and processing hardware. The design was developed with stability, compact dimensions and reliable steering in mind.

#### Material and Construction

#### Component Placement
The electronic components are arranged on several levels above the main chassis plate. The battery is positioned low inside the chassis, while the processing and control electronics are mounted above it. The camera is mounted at the front of the robot on a dedicated 3D-printed support. The distance sensors are positioned near the front of the vehicle so that they can detect the surrounding walls during navigation.

(gdje se nalaze no)
- Main controller: 
- Battery: 
- Drive motor: 
- Steering servo: 
- Sensors: 

#### Design Reasoning

The battery was positioned low in the chassis to keep the center of gravity as low as possible.
We placed X here because...
We chose X instead of Y because...
This reduced...
This improved...

#### Chassis Improvements

During testing, the distance sensors were positioned on the upper part of the robot. In this position, the sensors were too high and could not reliably detect the wall directly in front of the vehicle. After identifying this issue, we redesigned the sensor position and moved the distance sensors lower on the chassis. This improved their field of view and allowed them to detect the wall more reliably. This change showed us how strongly sensor placement can affect the performance of the navigation system.
<img src="media/development/version_2/build/build-03.jpeg" width="300">
<img src="media/development/version_2/build/build-04.jpeg" width="300">

| Original sensor position | Improved sensor position |
|---|---|
| <img src="docs/images/mechanical/lidar-before.jpeg" width="300"> | <img src="docs/images/mechanical/lidar-after.jpeg" width="300"> |

**OVO NE GINE NAPRAVIT**

before: wall missed in 4/10 runs
after: wall detected in 10/10 runs

### 5.2 Drive System

### 5.3 Steering System

The vehicle uses a servo-controlled front steering mechanism. A steering servo mounted at the front of the chassis moves a mechanical linkage that connects the two front wheels. Instead of controlling the left and right wheels with separate motors, both front wheels are mechanically linked and change direction together. This provides car-like steering while the rear axle provides propulsion. The steering components are mounted directly to the 3D-printed chassis, which allowed us to adjust the geometry and mounting positions during development.

<p align="center">
  <img src="media/development/version_2/final/bottom.jpeg" width="500">
</p>

<p align="center">
  <em>Front steering mechanism and mechanical linkage.</em>
</p>

### 5.4 Dimensions and Weight

| Measurement | Value |
|---|---|
| Length | TODO mm |
| Width | TODO mm |
| Height | TODO mm |
| Weight | TODO g |
| Wheelbase | TODO mm |
| Front track width | TODO mm |
| Rear track width | TODO mm |
| Front wheel diameter | TODO mm |
| Rear wheel diameter | TODO mm |

### 5.5 Torque / Speed Reasoning

### 5.6 Mechanical Testing and Iterations


## 6. Power & Sensor Architecture
### 6.1 Controller
### 6.2 Motors
### 6.3 Sensors
### 6.4 Sensor Placement
### 6.5 Wiring Diagram
### 6.6 Power Architecture
### 6.7 Sensor Calibration and Testing

## 7. Software Architecture
### 7.1 Overview
### 7.2 Program Structure
### 7.3 State Machine / Flowchart
### 7.4 Open Challenge Strategy
### 7.5 Obstacle Challenge Strategy
### 7.6 Control Algorithms
### 7.7 Edge Cases and Failure Handling

## 8. Engineering Decisions
### 8.1 Constraints
### 8.2 Design Trade-offs
### 8.3 Major Problems and Solutions
### 8.4 Why We Chose X Instead of Y

## 9. Testing & Results
### 9.1 Mechanical Tests
### 9.2 Sensor Tests
### 9.3 Open Challenge Tests
### 9.4 Obstacle Challenge Tests
### 9.5 Reliability Results
  
## 10. Components / Bill of Materials

[View the Bill of Materials PDF](docs/bill-of-materials/bill-of-materials.pdf)

## 11. Build & Reproduction Guide
### 11.1 Parts
### 11.2 Assembly
### 11.3 Wiring
### 11.4 Software Installation
### 11.5 Uploading / Running the Code

## 12. Repository Structure

## 13. Version History

## 14. Engineering Journal

## 15. Authors / Team
