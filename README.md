# Vision X - Real Time Object Counter  

Vision X is a **Streamlit-based web application** that leverages **YOLOv8** for real-time object detection and counting.  
It works with both **live webcam feeds** and **uploaded videos**, offering an interactive dashboard that shows detection results, object counts, and system performance metrics.

---

## 📌 Table of Contents
- [Features](#-features)  
- [Demo](#-demo)  
- [Requirements](#-requirements)  
- [Installation](#-installation)  
- [Usage](#-usage)  
- [Configuration](#-configuration)  
- [Project Structure](#-project-structure)  
- [Screenshots](#-screenshots)  
- [Credits](#-credits)  
- [License](#-license)  

---

## 🚀 Features
- Real-time **YOLOv8 object detection**  
- Support for **webcam input** and **uploaded videos** (MP4, AVI, MOV)  
- Adjustable **confidence threshold**  
- **GPU acceleration** (CUDA) support  
- Interactive **dashboard metrics**:  
  - Tracked Objects  
  - Frame Rate (FPS)  
  - Unique Classes Detected  
- Dynamic **object count table** with live updates  
- Customizable detection by selecting specific COCO classes  
- Clean UI with **custom CSS styling**  

---

## 🎥 Demo
Run locally with:
```bash
streamlit run app.py
```

When launched, open the link in your browser (default: [http://localhost:8501](http://localhost:8501)) to interact with the app.

---

## 🛠 Requirements

### Software

* Python **3.8+**
* [Streamlit](https://streamlit.io/)
* [PyTorch](https://pytorch.org/) (with CUDA for GPU acceleration, optional)
* [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
* OpenCV
* NumPy

### Python Dependencies

Install with:

```bash
pip install -r requirements.txt
```

Example `requirements.txt`:

```txt
streamlit>=1.36.0
opencv-python>=4.8.0
numpy>=1.24.0
ultralytics>=8.0.0
torch>=2.0.0
```

---

## 📦 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/vision-x.git
   cd vision-x
   ```

2. **(Optional) Create and activate a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Download YOLOv8 model**
   By default, the app uses `yolov8n.pt`. Ultralytics automatically downloads it on first run.

---

## ▶️ Usage

Run the app:

```bash
streamlit run app.py
```

* Use **Webcam** button for real-time detection
* Upload a **video file** (MP4/AVI/MOV) for processing
* Adjust confidence and toggle GPU in sidebar settings

---

## ⚙️ Configuration (Sidebar Options)

* **Confidence Threshold** → Filters out low-confidence predictions
* **Enable GPU** → Uses CUDA if available
* **Select Classes** → Choose which COCO object categories to detect
* **Input Source** → Webcam or uploaded video

---

## 📂 Project Structure

```
vision-x/
│── app.py              # Main Streamlit application
│── main.css            # Custom CSS styling
│── requirements.txt    # Python dependencies
│── README.md           # Project documentation
```

---

## 📸 Screenshots

### Main Dashboard

*(Example UI layout – Webcam/Video, Metrics, Object Counts)*
![Example UI](https://via.placeholder.com/800x400.png?text=Vision+X+Dashboard+Preview)

---

## 👨‍💻 Credits

Created with ❤️ by **Team Choice_Matrix**

* Built using [Streamlit](https://streamlit.io/)
* Powered by [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)

---

## 📜 License

This project is licensed under the **MIT License**.
You are free to use, modify, and distribute this project with attribution.

---
