# PDF-EXTRACTION-USING-PYTHON
This Python script allows us to automatically extract specific sections of text from PDF files based on keyword pairs. It's particularly useful for extracting structured sections from any pdf's.
What It Does:
Iterates over a folder of PDF files
Skips headers and footers to avoid noise
Locates text between specified start and end keywords
Extracts the matched content
Saves the results into a CSV file for easy analysis
How It Works:
fitz (PyMuPDF) is used to open and read PDF documents page by page.
Text is extracted block-wise and filtered to ignore headers/footers (based on vertical position).
For each PDF, it searches for text between the given start and end keyword pairs (case-insensitive).
The extracted snippets are collected and written to extracted_pdf_sections.csv.
Input Requirements:
Folder containing .pdf files
List of keyword pairs to define extraction boundaries
Output:
extracted_pdf_sections.csv containing:
File name
Start and end keywords
Extracted description between them
