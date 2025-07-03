# AI Document Assistant - Project README

## Overview
AI Document Assistant is a web application that enables users to upload, manage, and query documents using AI-powered natural language processing. The system uses Google's Gemini API to answer questions based on document content, providing both administrative and end-user interfaces.

## Key Features
- **User Authentication**: Secure login/registration system with role-based access (admin/user)
- **Document Management**:
  - Upload documents (PDF, DOCX, XLSX, PPTX)
  - View and delete uploaded files
- **AI Question Answering**:
  - Ask natural language questions about document content
  - Get AI-generated answers based on document context
- **Responsive UI**: Clean, modern interface with animations and hover effects
- **Role-Based Access**:
  - **Admin**: Full document management capabilities
  - **User**: Question answering interface only

## Technologies Used
- **Frontend**: HTML5, CSS3, JavaScript
- **Backend**: Python, Flask
- **AI Integration**: Google Gemini API
- **Document Parsing**: PyMuPDF, docx2txt, pandas, python-pptx
- **Storage**: Local file system for document storage
- **Authentication**: Session-based with JSON user storage

## Installation Guide

### Prerequisites
- Python 3.7+
- Pip package manager
- Google Gemini API key

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ai-document-assistant.git
   cd ai-document-assistant
