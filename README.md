#  **Fingerprint-Attendance-System**

##  Overview
The **Fingerprint-Attendance-System** is a biometric attendance solution that enables students to mark their attendance using a **fingerprint sensor** connected to an **ESP32 microcontroller**. The attendance records are automatically updated in **Google Sheets**, ensuring a paperless and efficient system.

This project aims to replace traditional manual attendance methods with a secure and automated system, reducing human error and enhancing reliability.

---

##  Features
✔️ **ESP32 & Fingerprint Sensor Integration** – Establishes communication between ESP32 and the fingerprint sensor.  
✔️ **Fingerprint Enrollment** – Allows students to register their fingerprints for authentication.  
✔️ **Google Sheets Integration** – Stores student names, roll numbers, and attendance records with timestamps.  
✔️ **Real-Time Authentication** – Matches fingerprints against stored data to verify student identity.  
✔️ **Automated Attendance Marking** – Updates Google Sheets upon successful authentication.  
✔️ **Error Handling** – Manages failed fingerprint matches, sensor errors, and connectivity issues.  
✔️ **Testing & Validation** – Ensures system reliability through rigorous testing.  

---

## Project Workflow  
1️⃣ **Setup ESP32 and Fingerprint Sensor** – Establish a stable connection.  
2️⃣ **Fingerprint Enrollment** – Store student fingerprints securely.  
3️⃣ **Google Sheets Integration** – Automate attendance logging.  
4️⃣ **Fingerprint Authentication** – Verify student identity.  
5️⃣ **Attendance Marking** – Automatically update attendance records.  
6️⃣ **Error Handling** – Manage exceptions and improve reliability.  
7️⃣ **Testing & Validation** – Optimize performance and ensure accuracy.  

---

## Hardware Requirements
- **ESP32 Microcontroller**  
- **Fingerprint Sensor (e.g., R307, GT511C3, etc.)**  
- **Jumper Wires**  
- **Power Supply (5V)**  
- **Laptop/PC for programming the ESP32**  

---

##  Software Requirements
- **Arduino IDE** (for writing and uploading code)  
- **Fingerprint Sensor Library** (Adafruit Fingerprint Sensor Library)  
- **Google Sheets API** (for logging attendance data)  
- **ESP32 Board Manager for Arduino IDE**  

---

## Installation & Setup

### 1️⃣ Install Required Libraries  
Open **Arduino IDE** and install the following libraries:
- **Adafruit Fingerprint Sensor Library** (via Library Manager)
- **WiFi Library** (for ESP32)
- **HTTPClient Library** (for Google Sheets integration)

### 2️⃣ Set Up ESP32 in Arduino IDE   
- To set up the **ESP32 in Arduino IDE**, you need to configure the environment by installing the necessary board definitions. 
- This involves adding the ESP32 package to the **Board Manager** and selecting the appropriate **ESP32 development module**. 
- Once configured, the Arduino IDE will be able to recognize and upload code to the **ESP32 microcontroller**.  

- Go to **Tools** → **Board** → **ESP32** → Select **ESP32 Dev Module**.

### 3️⃣ Set Up Google Sheets Integration  
- Enable **Google Sheets API** in the Google Cloud Console.  
- Generate **API credentials** and obtain the **Google Sheets API key**.  
- Share the Google Sheet with the generated API email.  

### 4️⃣ Upload the Code to ESP32  
- Connect ESP32 to your computer.  
- Open **Arduino IDE**, load the fingerprint attendance code, and upload it.  

---

##  Usage Guide

### 1️⃣ Enroll a New Fingerprint  
1. Run the enrollment script on ESP32.  
2. Place the student's finger on the sensor.  
3. The system will capture and store the fingerprint in memory.  

### 2️⃣ Mark Attendance  
1. The student places their finger on the sensor.  
2. If the fingerprint matches a stored record, attendance is marked in **Google Sheets**.  
3. If the fingerprint does not match, an error message is displayed.  

### 3️⃣ Check Attendance  
- Open **Google Sheets** to view attendance records, including **name, roll number, date, and time**.  

---

## Error Handling
- **Fingerprint Not Found** – Displays a message if the fingerprint does not match any stored records.  
- **Sensor Connection Issue** – Ensures proper wiring and sensor connection.  
- **Google Sheets API Failure** – Checks internet connectivity and API key.  

---

##  Future Improvements  
 **Cloud Database Support** – Integrate with Firebase for scalable attendance management.  
 **SMS/Email Notifications** – Send notifications for absentee students.  
 **Mobile App Interface** – Develop a mobile app for real-time monitoring.  

---


## Contact & Support  
📧 Email: **mehdiacademic512@gmail.com**  
📞 Contact Number: +923051212120
