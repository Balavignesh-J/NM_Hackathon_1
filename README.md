# 🎨 Color Tools - Streamlit App

A Streamlit web application that allows users to:
- Detect the name and RGB/HEX values of any color in an uploaded image by clicking on it.
- Visualize all predefined colors in a beautiful pie chart.

## 🔧 Features

### 🎯 Real-Time Color Detector
- Upload an image (`.jpg`, `.jpeg`, or `.png`).
- Click anywhere on the image to get:
  - Color Name
  - RGB Values
  - HEX Code
- Visual color preview box.

### 📊 Color Pie Chart
- Displays all color names from `colors.csv` as a pie chart.
- Each slice represents a color with its RGB values.
- Custom legend below the chart.

## 📁 Project Structure

```
.
├── main.py               # Main Streamlit application
├── colors.csv            # Color dataset (name, R, G, B)
└── piechart_colors       # Preset for pie chart rendering (optional)
```

## 🛠️ Requirements

- `Python 3.7+`
- `streamlit`
- `pandas`
- `numpy`
- `matplotlib`
- `Pillow`
- `streamlit-image-coordinates`

Install all dependencies using:

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available, install manually:

```bash
pip install streamlit pandas numpy matplotlib Pillow streamlit-image-coordinates
```

## 🚀 Run the App

```bash
streamlit run main.py
```

## 📷 Live Deploy

- [Streamlit link](https://nmhackathon1.streamlit.app/)

## 📄 License

This project is open-source and available for educational and personal use.
