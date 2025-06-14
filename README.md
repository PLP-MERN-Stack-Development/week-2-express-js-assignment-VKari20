# 📦 Product API – Express.js

A simple RESTful API built with Express.js for managing products.

---

## 🚀 Run the Server

1. Install dependencies:

   ```bash
   npm install
   
2. Create a .env file:
   PORT=3000
   API_KEY=your-secret-api-key

3. Start the server:
   node server.js

## 🧪 API Endpoints
All endpoints start with:
http://localhost:3000/api/products

## GET /
Welcome message.

## GET /api/products
 Get all products
✅ Supports ?category, ?page, ?limit

## GET /api/products/:id
Get product by ID

## POST /api/products
Create a product
🔐 Requires header: x-api-key

## Body:
{
  "name": "Phone",
  "description": "New smartphone",
  "price": 800,
  "category": "electronics",
  "inStock": true
}

## PUT /api/products/:id
Update product
🔐 Requires x-api-key

## DELETE /api/products/:id
Delete product
🔐 Requires x-api-key

## GET /api/products/search?name=term
Search products by name

## GET /api/products/stats
Return product stats






