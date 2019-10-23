# ocr
Simple OCR script that uses Google Drive's OCR capabilities.
To make it work do the following:

1. Visit https://developers.google.com/drive/api/v3/quickstart/python
2. Click Enable The Drive API
3. Login with your Google account
4. Click "Download Client configuration"
5. Copy the credentials.json to the same folder with ocr.py

Execution: Copy any files you need to convert in the same folder. Filetypes supported: pdf, jpg, png, gif, bmp, doc

python ocr.py

The script will list the supported files, upload each one to Google Drive and export/download the text version of them.

Example: original.jpg -> the exported will be original_jpg_text.txt, original.pdf -> the exported will be original_pdf_text.txt etc
