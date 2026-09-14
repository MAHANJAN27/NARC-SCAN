# NarcScan Proof of Concept (PoC)

## Overview
This repository contains the Python-based Proof of Concept for **NarcScan**, a cryptographically sealed offline field drug testing system. This computer vision engine was built to replace subjective visual inspections with mathematically verifiable digital evidence.

## Core Features Validated in this PoC:
* **Forensic Spatial Calibration:** Actively scans for physical ArUco markers and locks the system until alignment is achieved, neutralizing environmental variables.
* **Perceptual Color Engine:** Converts live webcam BGR pixel data into the CIE-L*a*b* color space to calculate exact chemical chromatic distances (Delta-E).
* **Secure Capture Logic:** Enforces a strict hardware lock, refusing to capture or save an evidence image unless the spatial and color parameters are met.

## Technology Stack Used
* Python
* OpenCV (cv2)
* NumPy
* OpenCV Aruco Module

## Current Status
**TRL 4 (Validated Proof of Concept):** The logic demonstrated in this Python script will be directly translated into Kotlin/CameraX for the final Android mobile application.
