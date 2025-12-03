# Car-Bluetooth-leak
**Passive Automotive Bluetooth OSINT Toolkit**  
Safe • Read-Only • No Pairing • No Exploitation

---

## 🔥 Overview

**BT-CAR Hacking Defalt** is a passive, read-only Bluetooth reconnaissance toolkit focused on automotive OSINT, BLE metadata analysis, and car-related signal intelligence.

It performs:

- Bluetooth Classic + BLE scanning  
- Automotive fingerprinting (global + Iranian cars)  
- BLE UUID-based car system detection  
- TPMS / OBD-II passive fingerprinting  
- Co-Channel BLE spectrum mapping  
- BLE Intent analysis  
- Radar (RSSI drift) movement tracking  
- Real-time triangulation (HTML)  
- RSSI waveform visualization  
- Metadata and advertisement logging  

This project is **fully safe**:  
No pairing, no PIN attempts, no writing, no brute force.

---

## ⚠ Legal & Safety Notice

BT-CAR is designed exclusively for:

- Research  
- Automotive security auditing  
- RF/BLE OSINT  
- Defensive and educational purposes  

This tool **does not**:

- Pair with devices  
- Attempt default PINs  
- Send packets or exploit ECUs  
- Write to any Bluetooth service  
- Perform intrusive operations  

All operations are **read-only BLE/Classic scanning**.

---

## ✨ Features

### ✔ Automotive Fingerprint Database (Global + Iran)
Includes BLE MAC OUIs and signatures for:

**Iran:**
- IKCO (Dena, Tara, Runna+)  
- SAIPA (Quick, Saina, Shahin)  
- Pars Khodro (Renault platform)  
- KMC Iran (X5/X7/K7 local assembly)  

**Global:**
- KMC / JAC / Chery  
- Hyundai / Kia  
- Toyota / Honda / Mazda / Nissan  
- BMW / Mercedes / Audi / VW  

### ✔ Strict Automotive UUID Verification (Mode B)
A device is classified automotive only if:

1. Its MAC prefix matches a known automotive vendor  
2. It broadcasts automotive BLE UUID clusters (e.g., `FFF0`, `180A`, `180F`)

Prevents false positives such as phones or BLE gadgets.

### ✔ OSINT Modules
- BLE Intent Engine (media sync, TPMS, OBD-II, etc.)
- Co-Channel Map (CH37/38/39 packet heatmap)
- Real-time RSSI triangulation (HTML output)
- Radar mode (RSSI drift → approaching / leaving)
- Waveform visual RSSI bars
- Metadata inspector
- Advertisement logger
- GATT dump (read-only)

---

## 📁 Output Structure
# BT-CAR Hacking Defalt  
**Passive Automotive Bluetooth OSINT Toolkit**  
Safe • Read-Only • No Pairing • No Exploitation

---

## 🔥 Overview

**BT-CAR Hacking Defalt** is a passive, read-only Bluetooth reconnaissance toolkit focused on automotive OSINT, BLE metadata analysis, and car-related signal intelligence.

It performs:

- Bluetooth Classic + BLE scanning  
- Automotive fingerprinting (global + Iranian cars)  
- BLE UUID-based car system detection  
- TPMS / OBD-II passive fingerprinting  
- Co-Channel BLE spectrum mapping  
- BLE Intent analysis  
- Radar (RSSI drift) movement tracking  
- Real-time triangulation (HTML)  
- RSSI waveform visualization  
- Metadata and advertisement logging  

This project is **fully safe**:  
No pairing, no PIN attempts, no writing, no brute force.

---

## ⚠ Legal & Safety Notice

BT-CAR is designed exclusively for:

- Research  
- Automotive security auditing  
- RF/BLE OSINT  
- Defensive and educational purposes  

This tool **does not**:

- Pair with devices  
- Attempt default PINs  
- Send packets or exploit ECUs  
- Write to any Bluetooth service  
- Perform intrusive operations  

All operations are **read-only BLE/Classic scanning**.

---

## ✨ Features

### ✔ Automotive Fingerprint Database (Global + Iran)
Includes BLE MAC OUIs and signatures for:

**Iran:**
- IKCO (Dena, Tara, Runna+)  
- SAIPA (Quick, Saina, Shahin)  
- Pars Khodro (Renault platform)  
- KMC Iran (X5/X7/K7 local assembly)  

**Global:**
- KMC / JAC / Chery  
- Hyundai / Kia  
- Toyota / Honda / Mazda / Nissan  
- BMW / Mercedes / Audi / VW  

### ✔ Strict Automotive UUID Verification (Mode B)
A device is classified automotive only if:

1. Its MAC prefix matches a known automotive vendor  
2. It broadcasts automotive BLE UUID clusters (e.g., `FFF0`, `180A`, `180F`)

Prevents false positives such as phones or BLE gadgets.

### ✔ OSINT Modules
- BLE Intent Engine (media sync, TPMS, OBD-II, etc.)
- Co-Channel Map (CH37/38/39 packet heatmap)
- Real-time RSSI triangulation (HTML output)
- Radar mode (RSSI drift → approaching / leaving)
- Waveform visual RSSI bars
- Metadata inspector
- Advertisement logger
- GATT dump (read-only)

---

## 📁 Output Structure

report/
└── DEVICE_NAME/
├── device_info.txt
├── advertisements.txt
├── gatt.txt
├── heatmap.txt
├── triangulation.html
└── DEVICE_NAME.html


---

## 🛠 Installation

### Debian / Ubuntu / Kali

```bash
sudo apt update
sudo apt install python3 python3-pip bluez bluez-tools
pip3 install bleak
OR
pip3 install bleak --break-system-packages
```
## Launch

python3 Exploit.py
