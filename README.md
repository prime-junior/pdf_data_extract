# PDF Data Extract

Python project to extract tabular data from automotive PDF files, separate relevant information (year, body code, engine size), and export to CSV/Excel for analysis.

## 📋 Project Overview


![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-work--in--progress-yellow)
![Project Status](https://img.shields.io/badge/status-work--in--progress-yellow?label=Project%20Status)
![Last Commit](https://img.shields.io/github/last-commit/weversonbarbieri/pdf_data_extract?color=blue)
![Issues](https://img.shields.io/github/issues/weversonbarbieri/pdf_data_extract)
![Pull Requests](https://img.shields.io/github/issues-pr/weversonbarbieri/pdf_data_extract)
![Stars](https://img.shields.io/github/stars/weversonbarbieri/pdf_data_extract?style=social)
![Forks](https://img.shields.io/github/forks/weversonbarbieri/pdf_data_extract?style=social)


This project automates the extraction of structured data from PDF documents, especially for multi-page documents with tables. The extracted data is cleaned, processed, and exported to CSV/Excel files.

**Main steps:**
 PDF reading
 Table extraction
 Data consolidation and cleaning
 Extraction of Year(s), Body Code(s), and Engine Size from the 'CALIBRATION' column and placement into new separate columns
 Export of processed data
 Further data manipulation and analysis (to be defined in the future)


## 🛠️ Technologies Used

- **Python 3.12**
- **pdfplumber** – PDF table extraction


## Features

- Extracts tabular data from multi-page automotive PDF files
- Separates and structures Year(s), Body Code(s), and Engine Size
- Cleans and consolidates tables
- Exports processed data to CSV/Excel
- Modular Jupyter notebooks for each extraction step


### Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd pdf_data_extract
   ```
2. Create and activate the virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate  # Windows
   # or
   source venv/bin/activate  # macOS/Linux
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```


## Folder Structure

```
pdf_data_extract/
├── LICENSE
├── README.md
├── requirements.txt
├── data/
│   ├── year_extracted.csv
│   ├── body_code_extracted.csv
│   ├── engine_size_extracted.csv
│   ├── data_extracted.csv
│   ├── part_number.pdf
├── notebook/
│   ├── body_code_extraction.ipynb
│   ├── new_pdf_extract.ipynb
│   ├── test.ipynb
│   ├── year_extraction.ipynb
```

## Author
Developed by [Weverson Barbieri de Oliveira](https://github.com/weversonbarbieri)

## License
MIT
