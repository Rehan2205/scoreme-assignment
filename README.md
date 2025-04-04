# 📄 Table Extraction from System-Generated PDFs

This project was built for a hackathon where the goal was to extract tabular data from **system-generated PDFs** (like account statements) **without using Tabula, Camelot, or image conversion**, and export the results to:

- 📊 **Excel Sheet** (`.xlsx`)
- 📄 **PDF** (`.pdf` in tabular format)

---

## 🚀 Features

- ✅ Detects tables in structured PDF documents using text extraction
- ✅ Extracts fields: `Date`, `Description`, `Amount`, `Balance`
- ✅ Cleans and formats data into neat tabular form
- ✅ Exports to:
  - `output_table.xlsx`
  - `output_table.pdf`
- ❌ **No** image conversion (no OCR)
- ❌ **No** third-party table tools (like Tabula, Camelot)

---

## 📁 File Structure

```
📦 your_project_folder/
├── main.py                 # Entry point to run the entire process
├── table_extractor.py      # Handles parsing tables from PDF
├── pdf_generator.py        # Converts the DataFrame to a styled PDF
├── requirements.txt        # Required packages
├── sample_input.pdf        # Input PDF (rename your input file to this)
├── output_table.xlsx       # Output Excel file
├── output_table.pdf        # Output formatted PDF table
└── README.md               # Project documentation
```

---

## 🛠️ Prerequisites

Ensure Python is installed (version >= 3.8 recommended).

Install required packages using:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

1. Place your system-generated PDF as `sample_input.pdf` in the project root.
2. Run the project:

```bash
python main.py
```

3. You’ll get two output files:
   - `output_table.xlsx`
   - `output_table.pdf`

---

## 📌 Instructions (from Hackathon Document)

- Input PDF is system-generated — no image/table borders.
- Extract content in structured table form.
- Avoid Tabula, Camelot, image-based techniques.
- Maintain accuracy of numeric and text fields.

---

## 🧪 Sample Input & Output

- Input: `test3.pdf`  
- Output Format Reference: `test6.docx`

---

## 🧰 Tools & Libraries Used

- [PyMuPDF](https://pymupdf.readthedocs.io/en/latest/) (for text extraction from PDFs)
- `pandas` (to structure and manage data)
- `reportlab` (to generate PDF tables)
- `openpyxl` (to write Excel files)

---


**Name:** Rehan Raza  
**Email:** *razarehan1999@gmail.com*  
**College:** Motilal Nehru National Institute of Technology Allahabad
