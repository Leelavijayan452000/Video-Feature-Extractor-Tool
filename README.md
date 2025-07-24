# Video-Feature-Extractor

The aim of this project is to develop a Python-based tool that can automatically extract key features from video files, such as scene transitions (shot cuts), average motion intensity, and presence of text content, using computer vision techniques like optical flow, histogram comparison, and OCR (Tesseract).

This tool can assist in video analysis, summarization, surveillance insights, and as a preprocessing step for video-based AI applications.


##  Features

| Feature              | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `shot_cuts`          | Number of significant scene changes using histogram difference              |
| `avg_motion`         | Average optical flow magnitude across frames                                |
| `text_present_ratio` | Ratio of frames containing meaningful text (OCR)                            |

---

##  Requirements

- Python 3.7+
- OpenCV
- NumPy
- pytesseract
- Tesseract-OCR (must be installed locally)

---

## How to Use 
1) Prepare Your input
   - Place your video file (e.g., sample.mp4) in the same folder as the Python script.    
2) Install Tesseract-OCR manually

   - Download: https://github.com/tesseract-ocr/tesseract

  After installing it, set the correct path:

```bash
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```
3) Add your Video
    - Place your .mp4 video fine
    
```bash
video_path = r"C:\Path\To\Your\Video.mp4"
```
4) Run the Notebook
    - Run the code "video_feture_ectractior.ipynb" using Jupyter Notebook or Jupyter Lab.
    - Make sure your video file path and Tesseract file is correct..

5) Output
    - Run the cell your output will appear in JSON format
