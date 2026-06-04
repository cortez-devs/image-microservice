# Image Microservice

A lightweight Node.js microservice for **image storage, retrieval, and deletion**.  
Designed for use in microservice‑based applications such as the **Family Meal Planner**.

This service accepts image uploads, stores them locally, and returns a unique ID that can be used to retrieve the image later.

---

## 🚀 Features

- Upload images via `POST /upload`
- Retrieve images via `GET /image/:id`
- Delete images via `DELETE /image/:id`
- Stores metadata in `data/images.json`
- Automatically manages the `/images` directory
- Simple, fast, and dependency‑minimal

---

## 📦 Installation

Clone the repository:

Install dependencies npm install

Start the server: node server.mjs

The service runs on: http://localhost:3000


---

## 📡 API Endpoints

### **1. Upload Image**
`POST /upload`

**Body:** `multipart/form-data`  
**Field name:** `image`

**Response:**
```json
{
  "message": "Image uploaded",
  "id": "1717430000000",
  "filename": "1717430000000.jpg"
}


