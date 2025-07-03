# AI Document Assistant - Project README

## 📖 Overview
**AI Document Assistant** is a web application that enables users to upload, manage, and query documents using AI-powered natural language processing. The system leverages **Google's Gemini API** to answer questions based on document content, with both administrative and user interfaces.

---

## 🔑 Key Features

- **User Authentication**: Secure login/registration with role-based access (admin/user)
- **Document Management**:
  - Upload documents (PDF, DOCX, XLSX, PPTX)
  - View and delete uploaded files
- **AI Question Answering**:
  - Ask natural language questions about document content
  - Get AI-generated answers based on context
- **Responsive UI**: Clean and modern interface with animations
- **Role-Based Access**:
  - **Admin**: Full document management and query access
  - **User**: Query-only access

---

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript
- **Backend**: Python, Flask
- **AI Integration**: Google Gemini API
- **Document Parsing**: `PyMuPDF`, `docx2txt`, `pandas`, `python-pptx`
- **Storage**: Local file system
- **Authentication**: Session-based with `users.json`

---

## 🚀 Features Summary

- ✅ User Registration and Login  
- ✅ Admin Dashboard for File Management  
- ✅ Document Upload (PDF, DOCX, PPTX, XLSX)  
- ✅ AI-powered Q&A from documents  
- ✅ Responsive and modern UI  
- ✅ Secure file parsing and session handling  
- ✅ Google Gemini 1.5 Flash integration  

---

## 📁 File Structure

```bash
project/
├── app.py                # Main Flask application
├── users.json            # User credentials store
├── uploads/              # Uploaded document storage
├── templates/
│   ├── index.html        # Login page
│   ├── register.html     # Registration page
│   ├── admin.html        # Admin dashboard
│   ├── user.html         # User interface
├── static/               # (Optional: for JS/CSS if extracted)
├── .env                  # API key configuration
```

---

## 🧪 Supported File Types

- `.pdf`  
- `.docx`  
- `.pptx`  
- `.xlsx`  

---

## 🔐 User Roles

- **Admin**: Upload, delete, and query documents  
- **User**: Query documents only (no upload/delete access)

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/ai-document-assistant.git
cd ai-document-assistant
```

### 2. Create virtual environment and install dependencies

```bash
python -m venv venv
source venv/bin/activate       # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Configure environment variables

Create a `.env` file in the root directory:

```ini
API_KEY=your_google_gemini_api_key
```

### 4. Run the application

```bash
python app.py
```

Then open: `http://localhost` in your browser.

---

## ✨ Usage

- Register as a user or login as `admin`.
- Admin users can upload and delete documents from the dashboard.
- All users can submit questions, and the assistant will return answers based on document content using the Gemini model.

---

## ✅ Admin Login

Use the username `admin` to log in with administrative privileges. Credentials are stored in `users.json`.

---

## 📌 Notes

- Gemini prompt context is truncated to 8000 characters to ensure fast and accurate responses.
- Sessions are managed using Flask's built-in session system.
- Only supported file types can be uploaded for security and parsing consistency.

---

## 🤝 Contributing

Contributions are welcome!  
Fork the repo → Make your changes → Submit a pull request ✅

---

## 📬 Contact

For feedback, questions, or support:  
📧 mchandru326@gmail.com
Or open an issue on the repository.
