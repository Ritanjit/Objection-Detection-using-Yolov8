# <picture><source srcset="https://fonts.gstatic.com/s/e/notoemoji/latest/1f4f8/512.webp" type="image/webp"><img src="https://fonts.gstatic.com/s/e/notoemoji/latest/1f50d/512.gif" alt="🔍" width="32" height="32"></picture> Multi-Model Object Detection using YOLOv8 


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PaIZxrfc-WmmDV99BEvk8mbvkzyprQ6-?usp=sharing)
[![Python](https://img.shields.io/badge/Python_3.10+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Ultralytics](https://img.shields.io/badge/YOLOv8-by_Ultralytics-green?logo=yolo)](https://github.com/ultralytics/ultralytics)
[![Gradio](https://img.shields.io/badge/Gradio-3.50+-orange?logo=gradio)](https://www.gradio.app)
[![Deploy on HF Spaces](https://img.shields.io/badge/Deploy-HF_Spaces-blue?logo=huggingface)](https://huggingface.co/spaces)


> **Project Description:**
> This project implements a visual comparison framework for object detection using three YOLOv8 models (Nano, Medium, Extra-large). It enables users to upload images and receive annotated detections from each model variant, displayed side-by-side for performance inspection through an interactive Gradio web interface.

## <picture><source srcset="https://fonts.gstatic.com/s/e/notoemoji/latest/1f680/512.webp" type="image/webp"><img src="https://fonts.gstatic.com/s/e/notoemoji/latest/1f4f7/512.gif" alt="📷" width="25" height="25"></picture> Sample Output

<table>
<tr>
  <td colspan="4" align="center">
    <strong>Comparison of Detection Results</strong>
  </td>
</tr>
<tr>
  <td align="center"><strong>Original Image</strong></td>
  <td align="center"><strong>YOLOv8n Detection</strong></td>
  <td align="center"><strong>YOLOv8m Detection</strong></td>
  <td align="center"><strong>YOLOv8x Detection</strong></td>
</tr>
<tr>
  <td align="center">
    <img src="https://raw.githubusercontent.com/Ritanjit/Objection-Detection-using-Yolov8/main/images/input.webp" width="250"/>
  </td>
  <td align="center">
    <img src="https://raw.githubusercontent.com/Ritanjit/Objection-Detection-using-Yolov8/main/images/yolov8n.webp" width="250"/>
  </td>
  <td align="center">
    <img src="https://raw.githubusercontent.com/Ritanjit/Objection-Detection-using-Yolov8/main/images/yolov8m.webp" width="250"/>
  </td>
  <td align="center">
    <img src="https://raw.githubusercontent.com/Ritanjit/Objection-Detection-using-Yolov8/main/images/yolov8x.webp" width="250"/>
  </td>
</tr>
<tr>
  <td colspan="4" align="center">
    <em>Each image is processed using 3 different YOLOv8 models for side-by-side comparison.</em>
  </td>
</tr>
</table>


## 📊 Dataset

* **Source:** COCO Dataset (pretrained on COCO 2017 via Ultralytics YOLOv8)
* **Input:** JPG/PNG images uploaded by users
* **Output:** Annotated images with bounding boxes, class labels, and confidence scores for detected objects


## <img src="https://raw.githubusercontent.com/Ritanjit/Objection-Detection-using-Yolov8/main/logo.png" width="22" height="22"/>  YOLOv8 Models Used

| Model       | Speed       | Size   | Accuracy | Use Case            |
|-------------|-------------|--------|----------|---------------------|
| YOLOv8n     | Fastest     | ~5 MB  | Lower    | Edge & real-time    |
| YOLOv8m     | Balanced    | ~22 MB | Medium   | General-purpose     |
| YOLOv8x     | Most Accurate | ~70 MB | Highest  | Accuracy-priority   |

Each uploaded image is processed by all 3 models and returned in a comparative layout.


## ⚙️ How to Use

### 🔧 Local Setup
```bash
git clone https://github.com/YOUR_USERNAME/yolov8-multi-model-detector.git
cd yolov8-multi-model-detector
pip install -r requirements.txt
python app.py  # Launches Gradio on localhost
```

### ☁️ Deploy via Hugging Face Spaces
```bash
gradio deploy
```


---


<div align="center">

Made with <picture><source srcset="https://fonts.gstatic.com/s/e/notoemoji/latest/2763_fe0f/512.webp" type="image/webp"><img src="https://fonts.gstatic.com/s/e/notoemoji/latest/2705/512.gif" alt="❤️" width="20" height="20"></picture> by [Ritanjit Das](https://github.com/ritanjit)

</div>
