# ocr
Simple OCR script that uses Google Drive's OCR capabilities.
To make it work do the following:

1. Visit https://developers.google.com/drive/api/v3/quickstart/python
2. Click Enable The Drive API
3. Login with your Google account
4. Click "Download Client configuration"
5. Copy the credentials.json to the same folder with ocr.py
6. install the following modules
 a. httplib2 (In windows 10 I executed python -m pip install httplib2 --user)
 b. apiclient (Win10: python -m pip install apiclient --user)
 c. Upgraded google-api-python-client (win10: python -m pip install --upgrade google-api-python-client --user)
 d. oauth2client (win10: python -m pip install oauth2client --user)

Execution: Copy any files you need to convert in the same folder. Filetypes supported: pdf, jpg, png, gif, bmp, doc

python ocr.py
On first run it will open your browser to verify permisions. If you see "This app isn't verified" ... click on Advanced and (IF YOU TRUST ME) click on Go to Quickstart (unsafe). Then click Allow and Allow. You can close the browser tab. The execution begins.

The script will list the supported files, upload each one to Google Drive and export/download the text version of them.

Example: original.jpg -> the exported will be original_jpg_text.txt, original.pdf -> the exported will be original_pdf_text.txt etc
