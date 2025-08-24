# projects
# My Awesome Project
# 📌 Multi-Robot Cooperative SLAM

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)  
[![ROS](https://img.shields.io/badge/ROS-noetic-green.svg)]()  
[![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)]()  

## 🌍 Overview
This repository provides an implementation of a **multi-robot cooperative SLAM system** designed for large-scale exploration under **bandwidth-limited communication**.  
The system enables multiple robots to collaboratively build consistent maps by exchanging **lightweight 2.5D submaps** and performing **sliding window optimization** for global consistency.  

Key features:
- 📡 **Low-bandwidth communication** via 2.5D submap exchange  
- 🧭 **Sliding window optimizer** for accurate and scalable pose graph optimization  
- 🤝 **Multi-robot cooperation** in distributed environments  
- 🛠️ **ROS-compatible** implementation with modular design  

---

## 🔑 System Architecture
```text
 ┌───────────────┐
 │   Robot A      │
 │  ┌──────────┐ │
 │  │ Local SLAM│ │
 │  └──────────┘ │
 │      │         │
 │  2.5D Submap   │
 └──────┼─────────┘
        │
  Low-bandwidth comm.
        │
 ┌──────┼─────────┐
 │   Robot B      │
 │  ┌──────────┐ │
 │  │ Local SLAM│ │
 │  └──────────┘ │
 │      │         │
 │  2.5D Submap   │
 └──────┼─────────┘
        │
        ▼
   Sliding Window Optimizer
        │
        ▼
   Global Consistent Map
