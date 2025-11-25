# Computer Vision Powered Image Search Engine using YOLOv11  
### *Object Detection–Driven Visual Search Application (Streamlit + YOLOv11)*

This project demonstrates a **computer vision–based image search engine** that identifies and retrieves images containing specific objects using **YOLOv11**, one of the latest and most accurate object detection models.  
The system analyzes a folder of images, detects objects within them, stores metadata, and enables **fast, content-based image retrieval**.  
A simple, interactive **Streamlit** interface makes the search experience smooth and user-friendly.


## Key Features

- Object detection powered by **YOLOv11m**  
- Supports **80 object categories** from the COCO dataset  
- Fast inference and metadata indexing for quick search  
- Streamlit-based web interface running locally  
- Optimized to run inside a Conda environment with GPU acceleration  
- Works with any user-provided folder of images  


## Dataset & Model Information

- **Dataset Used:** COCO Validation 2017 (500-image subset)  
- **Classes:** 80 COCO object categories  
- **Model:** `yolov11m.pt`  
- **Framework:** Ultralytics YOLO  

##  Environment Setup

### 1️ Create and Activate Conda Environment

```
conda create -n yolo_image_search_gpu python=3.11
conda activate yolo_image_search_gpu
```

### 2️ Install Required Dependencies (GPU-Optimized)

```
pip install "numpy<2" --force-reinstall --no-cache-dir
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu121
pip install opencv-python
pip install ultralytics
pip install streamlit
pip install pillow scipy psutil
```
### Running the Application

## Step 1 — Activate Environment

```
conda activate yolo_image_search_gpu
```

## Step 2 — Launch Streamlit App

```
streamlit run app.py
```

## How to Use the Application

1. Open the Streamlit interface

2. Choose "Process new images"

3. Enter the path to your image directory 

4. Provide the YOLO model weights path:

```
yolov11m.pt
```

5. Click Start Inference to process images

7. Use the search bar to query objects (e.g., person, car, dog, etc.)

8. View retrieved images that contain the requested object


### Summary

• The system efficiently detects objects across multiple images

• Object metadata is stored and indexed for fast retrieval

• The search interface returns relevant images instantly based on object names

• Demonstrates a scalable approach to content-based visual search using modern object detection

## Output

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/24d48699-3ccd-40df-bca1-71adf2dab236" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/357fbb4a-511c-40b0-b30d-80d4582d3275" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/85664eee-e056-47d8-b35d-683b7e5e9a07" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c96f9d09-5aeb-4202-b1a6-331cecd16e1b" />

## Result

This system successfully detects objects and retrieves relevant images based on object occurrences.
