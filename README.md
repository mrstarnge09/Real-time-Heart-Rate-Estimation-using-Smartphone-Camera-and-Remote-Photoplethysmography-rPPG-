# Heart Rate Estimation via Remote Photoplethysmography (rPPG)

This project implements a non-invasive, real-time Heart Rate (HR) estimation system using a standard smartphone camera. By leveraging **Remote Photoplethysmography (rPPG)**, the system detects subtle skin color variations caused by the cardiac cycle, even under dynamic lighting conditions.

## 🚀 Features

* **Real-time Monitoring**: Continuous pulse estimation from a video stream.
* **Hardware-Free**: Works with standard smartphone cameras or webcams; no wearable sensors required.
* **Robust Processing**: Utilizes skin-tone adaptive tracking and temporal filtering to mitigate motion artifacts and ambient light noise.
* **Signal Decomposition**: Employs ICA (Independent Component Analysis) or Chrominance-based processing to isolate the plethysmographic signal.

## 🛠️ Tools and Technologies

* **Programming Language**: Python 3.x
* **Computer Vision**: OpenCV
* **Numerical Processing**: NumPy, SciPy
* **Remote Capture**: IP Webcam (Android)

## 📁 Project Structure

* `main.py`: The primary entry point for the application.
* `modules/`: Contains logic for skin detection, signal filtering, and HR calculation.
* `docs/`: Project documentation and Review presentations.

## ⚙️ Setup and Installation

1. **Clone the repository**:
```bash
git clone https://github.com/yourusername/rPPG-Heart-Rate-Monitor.git
cd rPPG-Heart-Rate-Monitor

```


2. **Install dependencies**:
```bash
pip install opencv-python numpy requests scipy

```


3. **Android Camera Setup**:
* Install **IP Webcam** from the Play Store.
* Start the server in the app and copy the provided IP address.
* Update the `url` variable in `main.py` with your phone's IP (e.g., `http://192.168.1.5:8080/shot.jpg`).


4. **Run the application**:
```bash
python main.py

```



## 📅 Timeline (BCA Final Year Project)

* **Review I (Feb 2026)**: Problem Statement, Methodology, and initial environment setup.
* **Review II (Mar 2026)**: System Architecture and Module development.
* **Review III (Apr 2026)**: Final Implementation, Demo, and Results analysis.

## 📚 References

* McDuff, D. (2021). *Remote Photoplethysmography: A Survey*. IEEE Signal Processing Magazine.
* Poh, M. Z., McDuff, D. J., & Picard, R. W. (2010). *Non-contact, automated cardiac pulse measurements using video imaging and blind source separation*. Optics Express.
