# Deepfake Detection - Face Extraction & Dataset Preprocessing

## 🚀 Project Overview
This project is designed to preprocess video datasets for **deepfake detection** by extracting faces from videos, balancing the dataset, and preparing it for training. The pipeline efficiently detects faces using **MTCNN**, saves cropped images, and ensures an equal distribution of real and fake samples.

## 📌 Features
✅ **Face Extraction** - Extracts frames and detects faces using **MTCNN**.  
✅ **Dataset Preprocessing** - Crops and saves detected faces from real & fake videos.  
✅ **Class Balancing** - Ensures an equal distribution of images across both classes.  
✅ **Empty Folder Cleanup** - Removes unnecessary directories automatically.  
✅ **Optimized Performance** - Uses frame skipping and resizing for faster processing.  

## 🛠 Tech Stack
- **Python**
- **OpenCV** (for video processing & face cropping)
- **PyTorch** (for MTCNN face detection)
- **TQDM** (for progress tracking)
- **shutil & os** (for file management)


## 🔧 Installation & Setup
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/deepfake-detection.git
   cd deepfake-detection
   ```
2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```
3. **Prepare Your Dataset**
   - Place your real and fake videos in the `dataset/real` and `dataset/fake` folders respectively.

4. **Run Face Extraction**
   ```bash
   python extract_faces.py
   ```

5. **Balance the Dataset**
   ```bash
   python balance_dataset.py
   ```

## 🔍 How It Works
1. Reads video files from `dataset/real` and `dataset/fake`.
2. Extracts frames every **20 frames** to optimize processing.
3. Uses **MTCNN** to detect and crop faces.
4. Saves cropped faces in the `preprocessed_data/real` and `preprocessed_data/fake` folders.
5. Balances the dataset by removing excess images from the majority class.

## 🎯 Future Enhancements
- Train a deepfake detection model using Restnet50
- Improve face detection with advanced preprocessing techniques.
- Develop a web-based interface for deepfake detection.

## 📜 License
This project is licensed under the MIT License.

## 🤝 Contributing
Pull requests and suggestions are welcome! Feel free to fork and enhance the project.

## 📬 Contact
For queries or collaboration, reach out via logamanyan15@gmail.com
## Model Link
Create new folder named as model and placec this model inside
https://drive.google.com/file/d/1MwfsON3HNteK1aPxxbR95EDqskqgqYT9/view?usp=sharing



