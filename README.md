# File Metadata Microservice

A simple Node.js microservice that accepts file uploads and returns metadata including the file's name, type, and size.

## 🚀 Features

- Upload a file through an HTML form
- Receive metadata about the uploaded file:
  - File name
  - MIME type
  - File size in bytes

## 📦 Tech Stack

- Node.js
- Express.js
- Multer (middleware for handling file uploads)

## 📂 Project Structure

file-metadata-microservice/
├── public/
│ └── index.html # Frontend form for uploading files
├── server.js # Backend server logic
├── package.json



## 📥 API Endpoint

### `POST /api/fileanalyse`

**Request:**

- Form-data with file under the key `upfile`

**Response:**

```json
{
  "name": "myfile.png",
  "type": "image/png",
  "size": 12345
}
