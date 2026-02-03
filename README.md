Multidisciplinary engineer with graduate-level training focused on test systems, automation, and hardware–software integration. Experienced in designing and building lab-scale systems that bridge embedded electronics, mechanical hardware, and software control. Strong emphasis on design–build–test workflows, troubleshooting, and converting manual or fragile processes into repeatable, instrumented, and operator-friendly systems.

Background spans embedded systems, robotics integration, data acquisition, and rapid prototyping, with hands-on experience taking projects from concept through debugging and deployment. Particularly comfortable working at the boundary between physical hardware and control software, with a lab-to-production mindset grounded in practical constraints.

---

## Featured Projects

---

## Automated Laser Manufacturing Test Platform (Master’s Thesis)


::contentReference[oaicite:0]{index=0}


**Overview**  
A experimental apparatus designed to support research in surface processing of selective laser melting (SLM) 3D printed parts. This system replaced a manual, script-driven workflow with an integrated control solution using a SCAPS SAMlight software and USC-2 controller for laser and scan head control.

**Problem**  
The existing system required operators to manually run multiple scripts in sequence, creating opportunities for:
- Operator error  
- Inconsistent test conditions  
- Poor reproducibility  
- Inefficient experimentation  

**Solution**
- Automated test sequences using a unified control interface  
- Control of laser, scan head, and ancillary systems via SCAPS SAMlight software and USC-2 controller
- Improved and increased repeatability of test execution across users

**Technical Highlights**
- 3-axis galvanometer scan head, 1064nm ND-YAG fiber laser controlled through SAMlight
- Designed and machined custom kinematic coupling for repeatable sample positioning
- Integrated ancillary systems (Shielding gas, safety interlocks, etc) to USC-2 Controller
- Data acquisition through Keyence profilometer supporting surface roughness and morphology analysis  

**Tools & Technologies**
- Autodesk Fusion - 3D modeling
- Optical surface metrology (Keyence)
- Python - data processing and analysis
- SAMlight - laser and scan head control
- 3D printing (Formlabs Form4 for resin printing, various FDM printers)

---

## Industry 4.0 Automated Storage & Retrieval System (ASRS)


::contentReference[oaicite:1]{index=1}


**Overview**  
A lab-scale Automated Storage and Retrieval System (ASRS) with 100 physical storage locations, developed as part of an Industry 4.0 demonstration platform. The system was designed to replace manual part handling with a repeatable, software-controlled workflow, emphasizing reliability, traceability, and integration with upstream and downstream automation.

**System Capabilities**
- Automated storage and retrieval of small parts within a lab-scale manufacturing system
- Maintains a synchronized virtual storage model representing the state of 100 physical locations
- Implements first-available storage and retrieval logic to maximize throughput and reduce operator decision-making
- Supports manual override, homing, and recovery routines for debugging and fault isolation

**Technical Highlights**
- Hierarchical control architecture separating high-level logic from low-level motion control
- Raspberry Pi manages storage logic, system state, and ROS network communication
- Arduino Nano controls the carousel motion system using a rotary encoder and 12V DC motor
- Python-based virtual storage array synchronized with physical motion and robot actions
- Integrated Niryo Ned2 robot arm for automated transfer of parts to and from storage locations
- Networked into a larger ROS-based lab manufacturing system for coordinated operation


**Tools & Technologies**
- Raspberry Pi, Arduino Nano
- Python, Embedded C++
- ROS (system-level integration)
- Autodesk Fusion (custom mechanical components)

--- 


## Smart Plant Shelf


::contentReference[oaicite:3]{index=3}


**Overview**  
A Raspberry Pi–powered plant shelf that automates lighting and supports long-running time-lapse photography. The system adjusts day length and light intensity throughout the year and is designed to run unattended for extended periods, including clean startup and recovery after power loss. Time-lapse imaging provides a visible record of plant behavior and seasonal changes.
**System Capabilities**
- Automated lighting schedule based on calculated sunrise/sunset times
- Dynamic control of light intensity to simulate seasonal day changes
- Custom time-lapse image capture for capturing plant movement and visual changes (View on YouTube: https://www.youtube.com/@videosofstuffhappening)
- Automated startup and state recovery behavior after power loss

**Technical Highlights**
- Raspberry Pi–based control system running Python automation scripts
- High powered full-spectrum LED lighting system with DAC based dimming control
- Astronomical time calculations used to drive lighting schedules
- Debugging and hardening of startup scripts and background services for reliable unattended operation

**Tools & Technologies**
- Raspberry Pi
- Python
- Camera modules
- Constant current LED power supply

---

##Technical Capabilities

---

## 3D printing


::contentReference[oaicite:4]{index=4}


**Overview**  
Hands-on experience using FDM 3D printing as a rapid prototyping and iteration tool for functional parts, fixtures, enclosures, and mechanical upgrades. 3D printing is integrated into a broader design–build–test workflow, supporting embedded systems, automation projects, and mechanical experimentation.

**Capabilities and Experience**
- Design and fabrication of functional components for electronics enclosures, mechanical fixtures, and lab-scale systems
- Iterative testing and refinement of printed parts to evaluate fit, rigidity, thermal behavior, and durability
- Firmware configuration and tuning using Klipper, including motion control, acceleration limits, and custom macros
- Mechanical modification and troubleshooting of printers, including toolhead changes, frame stiffening, and power system upgrades

**Printer Platforms**
Sovol SV07
- Klipper-based system used to develop firmware-level understanding and custom G-code macros
- Implemented macros for acceleration stress testing, print-by-object workflows, and automated time-lapse capture

Monoprice Maker Select
- Converted to Klipper firmware
- Toolhead replaced with custom modified Prusa MK2S toolhead
- Frame brace modification for improved rigidity and print consistency

Monoprice MP10
- Controller upgrade to SKR Pico running Klipper firmware
- Electrical upgrade from 12V to 24V system
- Conversion from Bowden to direct-drive extrusion using BMG-style extruder and E3D V6 hotend
- 12V build plate heater replaced with 120V system with solid-state relay
- frame upgrade from V wheel bearings to linear rails
- Used for large-format functional prints (300mm x 300mm x 400mm build volume)

---

## Embedded Systems & Electronics Prototyping


::contentReference[oaicite:2]{index=2}


**Overview**  
Hands-on experience designing, building, and debugging embedded systems that integrate sensors, actuators, power electronics, and user interfaces. Projects emphasize practical constraints, iterative testing, and reliable operation, rather than proof-of-concept demos.

**Selected Systems & Prototypes**

Environmental filtration and ventilation controller for 3D printer enclosures
- Arduino Nano–based system integrating particulate matter, VOC, and temperature sensing
- PWM-controlled fan and variable air recirculation for basic thermal and airflow control
- HEPA13 and activated carbon filtration using readily available consumer air purifier filter elements
- Local system feedback via 12864 OLED display

Self-hosted home server for local services and data management
- Linux-based system providing media serving, file storage, and automated backups  
- Configured for multi-client access and long-running unattended operation  
- Used to support development workflows and data retention for personal projects  

Remote monitoring and actuation system (for pet rabbits)
- Raspberry Pi–based video monitoring
- Servo-driven automated feeder mechanism
- Relay-controlled lighting, integrating low-voltage control with switched loads

Battery powered temperature data logger
- Arduino-based system using DS18B20 digital temperature sensor
- Timestamped data logging to SD card
- Designed for untethered operation using 18650 battery power

**Common Technical Themes**
- Sensor integration and signal handling
- PWM motor and fan control
- Low-voltage power management and battery operation
- Local user interfaces (OLED displays)
- Debugging of embedded firmware and hardware interactions


---


## Automotive Diagnostics, Repair, and Performance Tuning


::contentReference[oaicite:5]{index=5}


**Overview**  
Professional experience diagnosing and repairing automotive systems in a dealership environment, with particular exposure to hybrid vehicles and electronically controlled powertrains. Additional personal experience exploring ECU calibration and performance tuning on privately owned vehicles.

**Professional Experience**
- Diagnostic and repair work performed as a dealership technician using OEM tools and procedures
- Use of manufacturer diagnostic software, including Subaru SSM and Toyota Techstream
- Hybrid vehicle high-voltage system diagnostics and safety-conscious repair practices
- Electrical and drivability troubleshooting using scan data, fault codes, and service documentation

**Personal Technical Projects**
- ECU data logging and calibration using ECUFlash and ROMRaider on a personally owned vehicle
- Software-based engine tuning resulting in approximately 30% power increase on a 2004 Subaru Impreza WRX
- Engine restoration and rebuild project on a Mazda Miata, including mechanical teardown, inspection, and reassembly  
- Hands-on exploration of engine management, fueling, ignition, and mechanical tolerances within safe operating limits

---


**Resume available upon request or via application portal**
**Email: joshfish9182@gmail.com**
