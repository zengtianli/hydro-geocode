# 📍 Hydro Geocode — Batch Geocoding Tool

[![GitHub stars](https://img.shields.io/github/stars/zengtianli/hydro-geocode)](https://github.com/zengtianli/hydro-geocode)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.36+-FF4B4B.svg)](https://streamlit.io)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-hydro--geocode.tianlizeng.cloud-brightgreen)](https://hydro-geocode.tianlizeng.cloud)

Batch geocoding tool using Amap (高德地图) API — convert addresses to coordinates and vice versa.

![screenshot](docs/screenshot.png)

## Features

- **Reverse geocoding** — convert lng/lat coordinates to detailed addresses
- **Forward geocoding** — convert addresses to lng/lat coordinates
- **Company search** — find company locations by name via POI search
- **WGS-84 ↔ GCJ-02 conversion** — automatic coordinate system transformation
- **Batch processing** — upload Excel/CSV, process hundreds of records
- **Built-in sample data** — try it instantly with included example files

## Quick Start

```bash
git clone https://github.com/zengtianli/hydro-geocode.git
cd hydro-geocode
pip install -r requirements.txt
export AMAP_API_KEY="your_key_here"
streamlit run app.py
```

## CLI Usage

```bash
# Reverse geocoding
python run.py reverse input.xlsx output.xlsx --gcj02

# Forward geocoding
python run.py address input.xlsx output.xlsx

# Company search
python run.py company input.xlsx output.xlsx
```

## Deploy (VPS)

```bash
git clone https://github.com/zengtianli/hydro-geocode.git
cd hydro-geocode
pip install -r requirements.txt
export AMAP_API_KEY="your_key_here"
nohup streamlit run app.py --server.port 8517 --server.headless true &
```

## Hydro Toolkit Plugin

This project is a plugin for [Hydro Toolkit](https://github.com/zengtianli/hydro-toolkit) and can also run standalone. Install it in the Toolkit by pasting this repo URL in the Plugin Manager. You can also **[try it online](https://hydro-geocode.tianlizeng.cloud)** — no install needed.

## License

MIT
