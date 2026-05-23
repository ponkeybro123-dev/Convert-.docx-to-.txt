# DOCX to TXT Converter

A simple web application that allows users to upload .docx files and convert them to plain text (.txt) format.

## Features

- 📁 Drag and drop file upload
- 🔄 Convert .docx files to .txt format
- 👀 Preview converted content
- ⬇️ Download the converted file
- 🎨 Beautiful and responsive UI
- ⚡ Fast conversion

## Requirements

- Python 3.7+
- Flask
- python-docx

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ponkeybro123-dev/Convert-.docx-to-.txt.git
cd Convert-.docx-to-.txt
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Start the Flask server:
```bash
python app.py
```

2. Open your browser and navigate to:
```
http://localhost:5000
```

3. Upload a .docx file by:
   - Clicking on the upload area to browse files
   - Or dragging and dropping a file

4. Click "Convert" to convert the file

5. Preview the content and download the .txt file

## Project Structure

```
Convert-.docx-to-.txt/
├── app.py              # Main Flask application
├── requirements.txt    # Python dependencies
├── templates/
│   └── index.html      # Web interface
└── uploads/            # Temporary upload folder (auto-created)
```

## How It Works

1. User uploads a .docx file through the web interface
2. Flask receives the file and validates it
3. The app uses `python-docx` library to extract text from:
   - Paragraphs
   - Tables
   - Other text elements
4. The extracted text is displayed as a preview
5. User can download the converted .txt file

## File Size Limit

- Maximum file size: 16MB

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python, Flask
- **File Processing**: python-docx

## License

MIT License

## Support

For issues or feature requests, please create an issue on GitHub.
