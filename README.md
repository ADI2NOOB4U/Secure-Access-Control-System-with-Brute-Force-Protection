# 🔐 Secure Access Control System with Brute Force Protection

A cybersecurity-focused embedded system project developed using Arduino in Tinkercad.  
This system implements PIN-based authentication and protects against brute-force attacks by enforcing automatic lockout and alarm triggering after multiple failed attempts.

---

## 🚀 Project Overview

This project simulates a secure physical access control system.  

The system:
- Accepts a 4-digit PIN via keypad
- Grants access by rotating a servo motor (door simulation)
- Tracks failed login attempts
- Detects brute-force behavior
- Locks the system after 3 incorrect attempts
- Activates buzzer and LED alarm during lockout

This models real-world authentication systems used in secure facilities and embedded access control devices.

---

## 🛠 Components Used

- Arduino Uno
- 4x4 Keypad
- 16x2 LCD Display (optional)
- Micro Servo Motor
- Buzzer
- LED
- 220Ω Resistor
- 10k Potentiometer (for LCD contrast)
- Breadboard & Jumper Wires

---

## 🔐 Security Features

- PIN-based authentication
- Failed attempt counter
- Brute-force detection
- Automatic system lockout (cooldown period)
- Alarm activation (LED + buzzer)
- Reset after timeout

---

## ⚙️ Pin Configuration

### Keypad
| Keypad Pin | Arduino Pin |
|------------|------------|
| R1 | 9 |
| R2 | 8 |
| R3 | 7 |
| R4 | 6 |
| C1 | 5 |
| C2 | 4 |
| C3 | 3 |
| C4 | 2 |

### Other Components
| Component | Arduino Pin |
|------------|------------|
| Servo Signal | 10 |
| Buzzer | 11 |
| LED | 12 |

---

## 🧠 Working Logic

1. User enters 4-digit PIN.
2. If PIN matches stored password:
   - Servo rotates to unlock position (90°).
   - Access granted.
3. If incorrect:
   - Failed attempt counter increments.
4. After 3 incorrect attempts:
   - System enters lockout mode.
   - LED and buzzer activate.
   - No input accepted for defined time period.
5. System resets automatically after cooldown.

---

## 🛡 Cybersecurity Concepts Demonstrated

- Authentication systems
- Brute-force attack mitigation
- Account lockout policy
- Intrusion detection
- Embedded system security
- Cyber-physical system protection

---

## 🔮 Future Improvements

- Encrypted PIN storage
- Admin override mode
- Attempt logging via Serial/Python
- IoT-based remote monitoring
- Multi-factor authentication
- RFID integration

---

## 📂 Project Structure

```
Secure-Access-Control-System/
│
├── arduino_code.ino
├── README.md
├── circuit_diagram.png
└── images/
```

---

## 👨‍💻 Author

Aditya Kumar Sharma  
Cybersecurity & Digital Forensics Student  
VIT Bhopal
