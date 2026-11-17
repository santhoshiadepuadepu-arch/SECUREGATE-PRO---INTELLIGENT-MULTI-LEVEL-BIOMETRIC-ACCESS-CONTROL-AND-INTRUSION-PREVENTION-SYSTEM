# 🔐 SecureGate Pro – Intelligent Multi-Level Biometric Access Control and Intrusion Prevention System

## 📌 Project Description

SecureGate Pro is an intelligent security and access control system developed using the **ARM7-based LPC2148 microcontroller**. The main objective of this project is to prevent unauthorized access by implementing a three-level authentication mechanism using **User ID, Password, and Fingerprint Recognition**.

The system verifies the user's identity at each authentication level before granting access. Only when all three verification stages are successfully completed will the door automatically unlock and open using a DC motor controlled by the L293D motor driver.

The project also provides administrator functionalities such as adding new users, deleting existing users, updating passwords, and enrolling or deleting fingerprints. User information and passwords are stored in external EEPROM memory (AT25C256).

If an unauthorized person attempts to access the system, it detects failed authentication attempts, generates security alerts, and maintains access logs through UART communication. This helps improve security, user management, and monitoring.

## 🎯 Objectives

- Implement three-level security authentication.
- Prevent unauthorized access using fingerprint verification.
- Provide secure user registration and management.
- Store user credentials in external EEPROM memory.
- Detect repeated incorrect password attempts.
- Automatically control door opening and closing.
- Monitor system activities through UART communication.

## ⚙️ Key Features

- **Three-Level Authentication:** User ID, Password, and Fingerprint.
- **Fingerprint Recognition:** Uses the R305 fingerprint module for enrollment and verification.
- **User Management:** Add and delete registered users.
- **Password Management:** Update passwords with confirmation.
- **EEPROM Storage:** Stores user details and password information.
- **Intrusion Prevention:** Detects repeated incorrect authentication attempts and locks the account.
- **Automatic Door Control:** Controls door movement using an L293D motor driver and DC motor.
- **UART Communication:** Sends authentication status and security logs to a PC.
- **LCD Display:** Displays authentication messages and system status.

## Block Diagram
<img width="620" height="339" alt="WhatsApp Image 2026-11-15 at 3 44 59 PM" src="https://github.com/user-attachments/assets/cd99ecd5-02f7-4741-8d0c-4937f82ec78e" />


## 🛠️ Hardware Requirements

- LPC2148 Microcontroller
- R305 Fingerprint Sensor Module
- 16×2 LCD Display
- AT25C256 EEPROM
- 4×4 Matrix Keypad
- MAX232 Communication Interface
- L293D Motor Driver
- DC Motor
- Push Button / Switch
- USB-to-UART Converter

## 💻 Software Requirements

- Embedded C Programming
- Keil µVision IDE
- Flash Magic
- Proteus (for circuit simulation, if applicable)

## 🔄 Working Principle

1. **User ID Verification:** The user enters their unique User ID through the keypad. The system checks whether the ID is registered.
2. **Password Verification:** The user enters the password. The system compares it with the password stored in EEPROM.
3. **Fingerprint Verification:** The R305 fingerprint module captures the fingerprint and compares it with the registered fingerprint templates.
4. **Access Granted:** If all three authentication levels are successful, the system grants access and activates the DC motor to open the door.
5. **Access Denied:** If any authentication stage fails, the system displays an error message on the LCD and denies access.
6. **Security Logging:** Authentication events and access status are transmitted to the PC through UART.


##Output
![Uploading IMG_20261103_170851020.jpg.jpeg…]()


## 👨‍💻 Administrator Functionalities

The administrator can access a separate menu to perform the following operations:

- Edit Password
- Edit Fingerprint
- Add New User
- Delete Existing User
- Exit Administrator Menu

## 🔌 Communication and Storage

- **UART:** Used to transmit authentication results, access logs, and system status to a PC.
- **EEPROM:** Used to store user IDs, passwords, and user records.
- **Fingerprint Module:** Stores and searches fingerprint templates for biometric authentication.

## 📊 Expected Results

- Successful authentication through all three security levels.
- Automatic door opening after successful verification.
- Access denial for invalid credentials or fingerprint mismatch.
- Detection of repeated incorrect password attempts.
- Secure user registration and deletion.
- Real-time system event monitoring through UART logs.

## 🚀 Applications

- Office and company security systems.
- Laboratory access control.
- Restricted-area security.
- Educational institutions.
- Secure rooms and server rooms.

## 📚 Conclusion

SecureGate Pro provides a reliable embedded security solution by combining password-based authentication with biometric fingerprint recognition. By integrating the LPC2148 microcontroller, EEPROM, keypad, fingerprint sensor, UART communication, and motor control, the system offers a multi-level approach to access control and unauthorized entry prevention.

**Technologies Used:** Embedded C | ARM7 | LPC2148 | UART | EEPROM | Fingerprint Recognition | LCD | Keypad | DC Motor Control
