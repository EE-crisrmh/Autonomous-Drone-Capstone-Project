# LumaWay 🌄

> **A GPS-guided autonomous drone system that guides lost hikers back to safety.**

---

## The Problem

Every year, thousands of hikers get lost on trails across the United States. Terrain looks the same in every direction. Cell service is gone. Panic sets in. Search and rescue teams can take hours to respond — and in the mountains, hours matter.

Current solutions require hikers to stay still and wait. LumaWay flips that. Instead of waiting to be found, the hiker gets found — and then guided home.

---

## What LumaWay Does

LumaWay is an autonomous drone system built for one purpose: get a lost hiker back on the trail.

Here's how it works:

1. **Before the hike**, the hiker opens the LumaWay app and starts a session. The app passively records their GPS trail as they walk in — no interaction needed, just like a fitness tracker running in the background.

2. **If they get lost**, they hit the SOS button. The app sends their current GPS location and their recorded trail path to the LumaWay ground station.

3. **The drone launches autonomously**, navigates to the hiker's GPS coordinates, and locates them.

4. **LumaWay leads them out.** The drone flies the recorded trail path in reverse — slowly, at walking pace — using a bright LED and audio signal to guide the hiker back to the trailhead. Follow the light. That's it.

No payload to drop. No complex robotics. Just a reliable, visible guide in the sky when you need it most.

---

## Why a Drone

A drone can cover terrain a person can't. It flies over downed trees, river crossings, and steep ridgelines. It doesn't get lost. It doesn't get tired. And it can reach a hiker in minutes rather than hours.

LumaWay isn't trying to replace search and rescue — it's a first response that buys time, reduces panic, and gets people moving in the right direction before conditions get worse.

---

## The System

LumaWay is built across three integrated components:

**Custom Flight Controller (Hardware)**
A 4-layer custom PCB built around dual STM32 microcontrollers — one for navigation, one for I/O. Onboard sensors include dual IMUs (ICM-20689, ICM-20602), a barometer (MS5611), and a magnetometer (IST8310) for full attitude and altitude awareness. Designed and manufactured in-house.

**Onboard Computing (Autonomy)**
An NVIDIA Jetson Nano handles high-level autonomy — GPS waypoint navigation, computer vision for hiker confirmation, and communication with the ground station over a wireless link.

**LumaWay App (Interface)**
A mobile app for hikers. Records the trail on the way in. Sends SOS with one tap. Shows the drone's live position on a map so rescue coordinators can monitor the situation in real time.

---

## Project Goals

- Demonstrate fully autonomous GPS-guided navigation to a target location
- Achieve stable hover and guided return-path flight in outdoor conditions
- Build a functional mobile app with trail recording and SOS capability
- Integrate onboard vision for hiker detection and confirmation
- Complete a full end-to-end demo: SOS sent → drone launches → hiker guided back

---

## Status

🔧 **In development** — UW Bothell Capstone Project, 2026–2027

---

## Team

Built by a four-person Electrical Engineering capstone team at the University of Washington Bothell, supervised by Dr. Hannachi.

- Cris R. Martinez Hernandez
- Abraham Chen
- Frank Ma
- Howard Sin

---

## Built With

- STM32F405 / STM32F103 (flight controller MCUs)
- NVIDIA Jetson Nano (onboard compute)
- T-Motor MN2806 Antigravity motors
- KiCad (PCB design)
- PlatformIO (firmware)
- Python / OpenCV (computer vision)
- React Native (mobile app)

---

*LumaWay — because everyone deserves a way home.*

