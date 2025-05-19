Below is the README in Markdown (.md) format, as requested. It’s a polished, professional, and concise description of the Streamlit-based Color Tools app, covering setup, usage, and functionality based on the provided code and dataset. The content is similar to the previous response but formatted explicitly as a standalone Markdown document.

```markdown
# Color Tools App

A Streamlit-based web application for exploring colors through two interactive tools: **Real-Time Color Detection** and **Color Pie Chart Visualization**. Built with Python, the app leverages a predefined color dataset (`colors.csv`) to detect colors in uploaded images or visualize colors in a pie chart.

## Features

- **Real-Time Color Detection**:
  - Upload an image (JPG, JPEG, PNG).
  - Click anywhere on the image to detect the closest matching color from the dataset.
  - Displays the color name, RGB values, HEX code, and a color swatch.
- **Color Pie Chart**:
  - Visualizes all colors from the dataset in a pie chart.
  - Each slice represents a color with its name and RGB values.
  - Includes a custom legend with color swatches.

## Dataset

The app uses `colors.csv`, which contains the following columns:
- `color_name`: Name of the color (e.g., Red, Green).
- `R`, `G`, `B`: RGB values (0–255) for each color.

Example:
```
color_name,R,G,B
Red,255,0,0
Green,0,255,0
Blue,0,0,255
...
```

## Prerequisites

- Python 3.8+
- Streamlit
- Required Python packages (listed in `requirements.txt`)

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Create a virtual environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Ensure the dataset**:
   - Place `colors.csv` in the same directory as `main.py`.

## Usage

1. **Run the Streamlit app**:
   ```bash
   streamlit run main.py
   ```

2. **Access the app**:
   - Open your browser and navigate to `http://localhost:8501`.
   - Use the sidebar to switch between "Color Detector" and "Color Pie Chart".

3. **Color Detector**:
   - Upload an image.
   - Click on the image to see the detected color's details (name, RGB, HEX, swatch).

4. **Color Pie Chart**:
   - View the pie chart of all colors in the dataset.
   - Check the legend for color names and RGB values.

## File Structure

- `main.py`: Main Streamlit application script.
- `colors.csv`: Dataset containing color names and RGB values.
- `requirements.txt`: List of required Python packages.

## Dependencies

Key libraries used:
- `streamlit`: For the web interface.
- `pandas`: For data handling.
- `numpy`: For color distance calculations.
- `PIL`: For image processing.
- `streamlit-image-coordinates`: For interactive image clicking.
- `matplotlib`: For pie chart visualization.

## Notes

- The app caches the color dataset for performance using Streamlit's `@st.cache_data`.
- The color detection uses Euclidean distance in RGB space to find the closest color match.
- Ensure uploaded images are in RGB format for accurate color detection.

## Contributing

Contributions are welcome! Please:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

## License

This project is licensed under the MIT License.