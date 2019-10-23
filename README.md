# ocr
Simple OCR script that uses Google Drive's OCR capabilities.
To make it work do the following:

Visit https://developers.google.com/drive/api/v3/quickstart/python
click Enable The Drive API
Login with your Google account
Click "Download Client configuration"
Copy the credentials.json to the same folder with ocr.py
Execution: Copy any files you need to convert in the same folder. Filetypes supported: pdf, jpg, png, gif, bmp, doc

python ocr.py

The script will list the supported files, upload each one to Google Drive and export/download the text version of them.

Example: original.jpg -> the exported will be original_jpg_text.txt, original.pdf -> the exported will be original_pdf_text.txt etc
