# UFLD Dashcam Lane Detection

Lane detection on dashcam video using the official **Ultra-Fast Lane Detection (UFLD)** implementation.

## Overview

This project applies the UFLD lane detection model on real-world dashcam footage. The pipeline performs model inference, decodes lane predictions, filters unwanted bonnet regions, and generates a final output video with detected lane points.

## Features

- Official UFLD PyTorch implementation
- Pretrained TuSimple lane detection model
- Custom dashcam video inference
- Lane prediction decoding
- Lane coordinate extraction
- Bonnet region removal
- Full video lane detection pipeline
- CUDA GPU acceleration

## Pipeline

The complete workflow includes:

1. Loading the pretrained UFLD model
2. Preparing dashcam video frames
3. Preprocessing frames for model input
4. Running lane detection inference
5. Decoding UFLD output into lane coordinates
6. Removing bonnet region from visualization
7. Applying lane detection on the complete video
8. Generating the final processed output video

## Requirements

Install all dependencies using:

```bash
pip install -r requirements.txt
```

A CUDA-enabled GPU is recommended for faster inference.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/ujalabasit7175/UFLD-Dashcam-Lane-Detection.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```
UFLD_Dashcam_Lane_Detection.ipynb
```

4. Run the notebook cells to perform lane detection on your dashcam video.

## Output

The system generates a processed video containing detected lane points overlaid on the original dashcam footage.

## Model

This project uses the pretrained TuSimple model from the official Ultra-Fast Lane Detection repository.

Official repository:

https://github.com/cfzd/Ultra-Fast-Lane-Detection

