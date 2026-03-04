# Kids Tablet Controller

**Remote control application for managing children's tablets from the vehicle's infotainment system.**

---

## 🎯 Overview

Kids Tablet Controller enables parents to remotely manage video playback and content on their child's tablet directly from the car's MMI interface, enhancing family safety and convenience during travel.

**Use Case:** Parents can control what their children watch on tablets in the backseat directly from the car's MMI screen, without needing to reach back or stop the vehicle while driving.

---

## ✨ Key Features

- **🎮 Remote Media Control**  
  Play, pause, next/previous controls from the driver interface

- **🔒 Safety Lockout**  
  Automatic UI restrictions during vehicle movement using VHAL speed data

- **📡 Local Network Communication**  
  WebSocket-based communication via vehicle WiFi hotspot

- **🔐 Privacy First**  
  No internet required for core functionality - everything works offline

- **👨‍👩‍👧 Family-Friendly Design**  
  Interface optimized specifically for in-vehicle family use

- **🌙 Day/Night Mode**  
  Automatic theme switching based on vehicle settings

---

## 🏗️ Technical Architecture

### MMI Controller App
- Native Android Automotive OS (AAOS) application
- Large, touch-friendly UI optimized for in-car use
- WebSocket client for communication
- VHAL integration for vehicle data (speed, day/night mode, parking brake)
- mDNS service discovery for automatic device pairing

### Tablet Client App
- ExoPlayer-based video player
- WebSocket server for receiving commands
- Content library management
- Offline playback support

### Communication
- **Protocol:** WebSocket over local network
- **Discovery:** mDNS (Network Service Discovery)
- **Transport:** Vehicle WiFi hotspot (infrastructure mode)
- **No cloud dependency:** All communication is local

---

## 🚗 Target Platform

- **Primary:** Ready Link Marketplace (HARMAN Ignite)
- **Vehicles:** VW Group (Audi, Volkswagen, etc.) with Android Automotive OS
- **Tested on:** 2026 Audi Q3 with Android 13
- **Requirements:** Android Automotive OS 13+ (MMI), Android 10+ (Tablet)

---

## 📋 Development Status

**Current Phase:** Development & Testing

- ✅ Architecture design complete
- ✅ Technical specifications defined
- ✅ Ready Link Marketplace registration in progress
- 🔄 Development on automotive emulator
- 🔄 Testing on target hardware
- ⏳ Submission to HARMAN for certification

---

## 🛠️ Technology Stack

**MMI App:**
- Kotlin
- Jetpack Compose
- Android Automotive Car API
- OkHttp (WebSocket)
- Android NSD (mDNS)

**Tablet App:**
- Kotlin
- ExoPlayer
- OkHttp (WebSocket)
- Material Design 3

---

## 🎯 Use Cases

1. **Long Road Trips**  
   Parents can queue up educational content or movies without stopping

2. **Safety During Driving**  
   UI automatically locks when vehicle is moving to prevent distractions

3. **Content Management**  
   Easy selection of age-appropriate content from the driver's seat

4. **Offline Entertainment**  
   Pre-loaded content works without internet connection

---

## 📱 Screenshots

*Coming soon - Development in progress*

---

## 🔐 Privacy & Safety

- **No Data Collection:** App does not collect or transmit personal data
- **Local Operation:** All functionality works without internet
- **Safety First:** Respects driver distraction guidelines
- **Parental Control:** Parents maintain full control over content

---

## 📞 Contact

**Developer:** Dmytro Gridchyn
**Email:** filler-fishery1g@icloud.com 
**Country:** Poland  
**Platform:** Ready Link Marketplace  

For partnership inquiries or questions, please reach out via email.

---

## 📄 License

Personal/Educational Project  
© 2026 Dmytro Gridchyn

---

## 🚀 Roadmap

- **Q1 2026:** Development & testing on emulator
- **Q2 2026:** HARMAN certification
- **Q2 2026:** Audi/VW OEM approval
- **Q3 2026:** Public release on Ready Link Marketplace

---

*This application is being developed for submission to the Ready Link Marketplace and HARMAN Ignite ecosystem for VW Group vehicles.*
```
