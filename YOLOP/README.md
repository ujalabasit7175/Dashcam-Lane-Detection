# YOLOP Dashcam Lane Detection

Real-time lane detection on dashcam video using the official **YOLOP (You Only Look Once for Panoptic Driving Perception)** implementation.

## Overview

This project applies the official YOLOP model on real-world dashcam footage for road scene understanding.

YOLOP is designed for autonomous driving perception and performs multiple tasks including:
- Lane detection
- Drivable area segmentation
- Object detection

In this project, the focus is on applying YOLOP for lane detection on dashcam video.

## Features

- Official YOLOP implementation
- Pretrained YOLOP model
- Dashcam video inference
- Lane detection visualization
- GPU accelerated inference
- Processed output video generation

## Pipeline

The workflow includes:

1. Cloning the official YOLOP repository
2. Installing required dependencies
3. Loading pretrained YOLOP weights
4. Running inference on dashcam video
5. Generating lane detection output
6. Converting output video into a compatible format
7. Exporting the final processed video

## Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

A CUDA-enabled GPU is recommended for faster inference.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/hustvl/YOLOP.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run inference:

```bash
python tools/demo.py \
--source dashcam_video.mp4 \
--weights weights/End-to-end.pth \
--img-size 640
```

4. The processed output video will be generated in:

```
inference/output/
```

## Output

The final output contains the detected lane regions overlaid on the original dashcam footage.

## Model

This project uses the official YOLOP pretrained model.

Official repository:

https://github.com/hustvl/YOLOP

## Notes

The pretrained YOLOP model was used directly for inference. No additional training or fine-tuning was performed in this project.
