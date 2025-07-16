

# 🎨 Real-Time Cartoonify with OpenCV

This Python application captures live video from your webcam and applies a **cartoon effect** to each frame using OpenCV. The result is displayed in real-time alongside the original feed.

---

## 📸 Demo

Two windows will open when you run the app:

- 🟦 **Original** – The live feed from your webcam.
- 🟨 **Cartoonified** – The same feed with a cartoon filter applied.

Press `q` to exit the program.

---

## 🧠 How It Works

The cartoon effect is achieved using a combination of image processing techniques:

1. **Grayscale Conversion** – Simplifies the image by removing color.
2. **Median Blur** – Reduces image noise.
3. **Edge Detection** – Uses adaptive thresholding to find edges.
4. **Bilateral Filter** – Smooths colors while preserving edges.
5. **Bitwise AND** – Combines the smooth image with edges to produce a cartoon effect.


````markdown


 📂 Project Structure

cartoonify/
│
├── cartoonify_webcam.py   # Main application file
├── requirements.txt       # List of dependencies
└── README.md              # You're reading this!
````

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/cartoonify.git
cd cartoonify
```

### 2. Set Up a Virtual Environment (Optional but recommended)

```bash
python -m venv venv
source venv/bin/activate    # On Windows use: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the App

```bash
python cartoonify_webcam.py
```

Press `q` to exit the video window.

---

## 🧾 Requirements

* Python 3.6+
* OpenCV (Python bindings)

See `requirements.txt` for exact versions.

---

## ⚙️ requirements.txt

```text
opencv-python
```

---

## 📌 Notes

* Ensure your webcam is accessible and not being used by another app.
* Works cross-platform (Windows, macOS, Linux).
* For headless environments (e.g. servers), use `opencv-python-headless`.



