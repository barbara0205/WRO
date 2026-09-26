# MechaMinds-WRO 2026 Future Engineers
# WRO Future Engineers - Engineering Documentation
# Team Members
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
Our project is an autonomous vehicle that can navigate the competition field, detect and avoid obstacles, follow the track and make real time decisions without human intervention.

## 2. Team
We are Croatia robotics team **MechaMinds** and our names are **Barbara Lukić**, **Ivano Koren** and **Nadia Kravčuk**. We come from high school Tin Ujević in Kutina. Our mentors name is Damir Petravić. Together we worked on design of the robot, programming and testing our robot.

## 3. Vehicle Overview
| Specification | Value |
|---|---|
| Length | 18 cm |
| Width | 17,5 cm |
| Height | 15,5 cm |
| Weight | _ |
| Drive type | Rear-wheel drive |
| Steering type | Ackermann steering |     ---Servo-controlled front steering???
| Main controller | Raspberry Pi 5 Model (B Rev1.1) |
| Programming language | C++ |
| Main sensors | MRMS LIDAR 2 m (VL53L0CX), CAN Bus |
| Camera | Raspberry Pi Camera Module 3 |
| Power source | 11.1 V, 5000 mAh (55.5 Wh) battery |

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

### 4.5 Current Robot
The robot we are using for competition in Zagreb will be [4.2 Version 2](#42-version-2) 


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


<img src="media/development/version_2/build/build-03.jpeg" width="250">  <img src="media/development/version_2/build/build-04.jpeg" width="250">

**Test result:**
| Sensor position | Successful wall detections |
|---|---:|
| Original higher position | 4/10 |
| Lowered position | 8/10 |
????????????

### 5.2 Drive System

**TU TREBA SLIKA OD DOLJE I ZADNJI KOTACI (POGON)**

### 5.3 Steering System

The vehicle uses a servo-controlled front steering mechanism. A steering servo mounted at the front of the chassis moves a mechanical linkage that connects the two front wheels. Instead of controlling the left and right wheels with separate motors, both front wheels are mechanically linked and change direction together. This provides car-like steering while the rear wheels make the robot move forward. The steering components are mounted directly to the 3D-printed chassis, which allowed us to adjust the geometry and mounting positions during development.

<p align="center">
  <img src="media/development/version_2/final/bottom.jpeg" width="500">
</p>

<p align="center">
  <em>Front steering mechanism and mechanical linkage.</em>
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
## Connection Failure 

- During development, we experienced repeated problems with the Wi-Fi connection between the robot and the development computer. The connection was unstable and we could not work with the robot properly. To improve reliability, we tested a wired Ethernet connection using an RJ45 network cable. During our tests, this connection proved to be significantly more stable and reliable than Wi-Fi, so we decided to use the wired connection during development.

<img src="media/connection-solution/connection1.jpeg" width="200"> <img src="media/connection-solution/connection2.jpeg" width="200">
<img src="media/connection-solution/connection3.jpeg" width="200"> <img src="media/connection-solution/connection4.jpeg" width="200">

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


