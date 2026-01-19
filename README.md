# PDF Data Extract

A Python project for extracting tabular data from PDF files and converting it to Excel format for further analysis.

## 📋 Project Overview

This project automates the extraction of structured data from PDF documents, specifically designed to handle multi-page documents with tabular information. The extracted data is cleaned, processed, and exported to Excel format.

## 🛠️ Technologies Used

- **Python 3.12**
- **pdfplumber** - PDF table extraction
- **pandas** - Data manipulation and cleaning
- **Jupyter Notebook** - Interactive development environment

## 📁 Project Structure

```
pdf_data_extract/
├── pdf_extract.ipynb     # Main notebook with extraction logic
├── pdf.pdf              # Source PDF file (ignored in Git)
├── .gitignore           # Git ignore configuration
├── README.md            # Project documentation
└── venv/                # Python virtual environment
```

## 🚀 Getting Started

### Prerequisites

- Python 3.12
- Virtual environment (recommended)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd pdf_data_extract
```

2. Create and activate virtual environment:
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install pdfplumber pandas jupyter
```

### Usage

1. Place your PDF file in the project directory and name it `pdf.pdf`
2. Open Jupyter Notebook:
```bash
jupyter notebook
```
3. Run `pdf_extract.ipynb` cells sequentially
4. The cleaned data will be exported as `chrysler_pdf_to_excel.xlsx`

## 📊 Data Processing Workflow

1. **PDF Reading** - Opens and loads PDF document
2. **Table Extraction** - Extracts tabular data from each page
3. **Data Consolidation** - Combines data from all pages
4. **Data Cleaning**:
   - Removes duplicate headers
   - Filters rows containing 'CALIBRATION' keyword
   - Drops unnecessary columns (TSB(S), RECALL(S))
   - Formats text (removes line breaks)
5. **Excel Export** - Saves processed data to Excel file

## Author
Developed by [Weverson Barbieri de Oliveira](https://github.com/weversonbarbieri)

## License
MIT

