"# PDF-to-Excel-Extractor"
```markdown
# MERN PDF Table Extractor

## Overview

MERN PDF Table Extractor is a full-stack web application that allows users to upload PDF files, extract tabular data, and download the extracted data in Excel format.

## Features

-  PDF Upload  files via drag-and-drop or file selection.
- Extract tables from PDFs using regex.
- Download extracted data as an Excel file.
- Uses MongoDB for storing extracted data.

## Tech Stack

- **Frontend**: React.js, Bootstrap, Axios, React Dropzone
- **Backend**: Node.js, Express.js, Multer, PDF-Parse, pdf2pic, XLSX, CORS
- **Database**: MongoDB with Mongoose
- **Libraries Used**: `axios`, `pdf-parse`, `tesseract.js`, `exceljs`, `multer`, `mongoose`

## Installation and Setup

### Prerequisites

- Node.js installed
- MongoDB installed and running locally or on a cloud service (e.g., MongoDB Atlas)

### Backend Setup

1. Navigate to the backend folder:
   ```sh
   cd backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3.  PORT=3000

4. Start the backend server:
   ```sh
   npm start
   ```

### Frontend Setup

1. Navigate to the frontend folder:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the React app:
   ```sh
   npm start
   ```

### Running the Project

1. Start the backend server (`npm start` in the `backend` folder).
2. Start the frontend (`npm start` in the `frontend` folder).
3. Open `http://localhost:3000` in your browser.

## API Endpoints

| Method | Endpoint        | Description               |
|--------|---------------|---------------------------|
| POST   | `/api/upload` | Upload and process PDF    |
| GET    | `/api/data`   | Get extracted table data  |
| GET    | `/api/download/:filename` | Download the generated Excel file |


