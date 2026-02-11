---


https://huggingface.co/spaces/pavellakov/simple-data-dashboard


---

# Simple Data Dashboard (Streamlit)

A lightweight Streamlit dashboard for exploring a CSV file: preview, summary stats, filtering, and a quick line chart.

## Features
- Upload any `.csv` file
- Preview the first rows
- Summary statistics (`describe()`)
- Filter rows by selecting:
  - a column
  - a value from that column
- Generate a simple line chart using selected X and Y columns (on the filtered data)

## Tech Stack
- Python
- Streamlit
- Pandas / NumPy
- Matplotlib (imported; Streamlit chart used for the plot)

## Run Locally

### 1) Create a virtual environment (recommended)
```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
# .venv\Scripts\activate  # Windows
```

### 2) Install dependencies
```bash
pip install streamlit pandas numpy matplotlib
```

### 3) Start the app
```bash
streamlit run app.py
```

Then open the local URL shown in the terminal (usually http://localhost:8501).

## Project Structure (suggested for GitHub)
```
simple-data-dashboard/
  main.py
  README.md
  requirements.txt
```

### Example `requirements.txt`
```txt
streamlit
pandas
numpy
matplotlib
```

## Tips
- For best results, pick numeric columns for the Y-axis.
- If your X column is not unique or not sorted, the line chart may look messy—try using an index-like column.

## License
Add a license if you plan to publish publicly (MIT is common for small demo projects).
