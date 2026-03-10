# Vitamin Bottle Tracking - Viam

## What this project does
This project uses a laptop webcam and Viam's AI platform to detect 
and track a Kirkland Adult Multivitamin Gummies bottle in real time 
using a custom trained object detection model.

## Hardware Used
- Windows PC/Laptop
- Built-in laptop webcam

## Software Used
- [Viam](https://app.viam.com) — robotics and AI platform
- modular-webcam by viam-labs — Windows webcam driver
- TFLite CPU — model inference engine

## How it works
1. Webcam captures live video feed
2. Custom trained TFLite model detects the bottle in each frame
3. Bounding box is drawn around the bottle with a confidence score
4. Only detections above 50% confidence are displayed

## Setup
1. Create a machine on app.viam.com
2. Install viam-server on Windows
3. Paste `config.json` into the JSON configuration tab
4. Save and wait for the machine to go Live

## Known Limitations
- Detection accuracy decreases at far range
- Requires good lighting for best results

## What I learned
- How to configure a webcam on Windows using Viam
- How to capture and label training data
- How to train and deploy a custom object detection model
- How to run real time AI inference on a live camera feed
