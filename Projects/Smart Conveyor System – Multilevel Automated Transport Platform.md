# Smart Conveyor System – Multilevel Automated Transport Platform

This project simulates a **six-level automated transport system**, designed to manipulate and transfer objects between different platforms through a **360° rotating base**, **conveyor belts**, and a **robotic gripper controlled from a web interface**.

It combines **mechatronics, motion control, and IoT connectivity** using an **ESP32** with WiFi connection, offering a functional demonstration of how automated systems can integrate into smart industrial environments.

---

## Project Objective

Develop a **functional automated transport model** capable of:
- Picking up objects from a conveyor belt  
- Rotating the main platform to different levels  
- Placing objects at designated positions  
- Being remotely controlled through a **web page** hosted on the ESP32  

---

## Main Components

| Type | Component | Function |
|------|------------|-----------|
| Controller | **ESP32 with WiFi** | Main controller and web server |
| Actuator | **Stepper Motor** | 360° rotation of the main base |
| Actuator | **2 DC Motors** | Drive the conveyor belts |
| Actuator | **Servo Motor** | Opens and closes the gripper |
| Actuator | **DC Motor** | Controls the extension and retraction of the gripper shaft |
| Power Control | **2 H-Bridges (L298N or similar)** | Control of DC motors |
| Step Control | **Stepper Motor Driver** | Stepper motor management |
| Display | **LCD Screen with I2C Module** | Shows the system IP address |
| Software | **Embedded Web Server (HTML + JS)** | Remote control interface |

---

## System Description

The system consists of **six levels**, of which **two are active conveyor belts** and the remaining are static platforms.  
A **rotating base** allows precise positioning of the gripper over each level, while the **robotic gripper** performs the object manipulation tasks.

All **system control** is handled through a **web interface hosted on the ESP32**, allowing execution of individual or automated sequences.

---

## General Operation

1. When powered on, the **LCD screen** displays the connection IP address.  
2. The user accesses the web interface via browser and selects commands.  
3. The ESP32 sends control signals to the **drivers and H-bridges**.  
4. The **rotating base** positions the gripper at the desired level.  
5. The **gripper** picks up the object and deposits it at another level or conveyor.  
6. The sequence can be repeated or automated through predefined routines.

---

## Applied Technologies and Concepts

- Control of **DC, servo, and stepper motors**  
- **WiFi communication** through ESP32 embedded server  
- Integration of **hardware and software in real-time**  
- Data display using **LCD + I2C module**  
- Modular and scalable design for industrial applications  

---

## Project Images

<div align="center">
  <img width="563" height="544" alt="image" src="https://github.com/user-attachments/assets/2e0ee54d-66d1-4582-9064-59b629d369d9" />
  <img width="316" height="748" alt="image" src="https://github.com/user-attachments/assets/75d59a5c-482e-40d6-bb7e-7b34b9a85a80" />
  <img width="502" height="932" alt="image" src="https://github.com/user-attachments/assets/faf1c97e-cf3f-4257-8aef-a66ae87240d5" />
  <img width="498" height="910" alt="image" src="https://github.com/user-attachments/assets/ea2649ff-0f94-4bb7-8c9d-92e349704ac5" />
</div>

---

## Future Improvements

- Implement **PID control** for optimized movements  
- Integrate **proximity or vision sensors** for object detection  
- Add **data logging and IoT monitoring** to external platforms  
- Develop a **mobile app** for remote control  

---

## Author

**Karla Barón**  
Mechatronics Engineer and Biomedical Engineer  
Colombia  

**Contact:**  
📧 karla.baron.39@gmail.com  
📱 +57 305 384 7166  
