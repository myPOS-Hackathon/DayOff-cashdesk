# Secure POS App

A lightweight Point of Sale (POS) application built with React for quick retail-style checkout. Great for hackathons, demos, or small store setups.

## Features

- Product listing from JSON
- Add/remove items to cart
- Calculates total
- Sends total (in cents) to backend via API
- Displays styled success/failure messages

## Folder Structure

```
simple-pos/
├── public/
│   └── index.html
├── src/
│   ├── data/
│   │   └── products.json
│   ├── App.js
│   ├── App.css
│   └── index.js
├── package.json
└── README.md
```

## How to Run

### 1. Install dependencies
```bash
npm install
```

### 2. Start the frontend (React app)
```bash
npm start
```
Opens at: `http://localhost:3000`

### 3. (Optional) Start mock backend server
If using the mock API server:
```bash
node server.js
```

Server will listen at: `http://localhost:4000/api/pay`

## API Contract
POST `/api/pay`
```json
{
  "amount": 1999
}
```
Response:
```json
{
  "message": "Payment of 1999 processed."
}
```

## Notes
- Total is sent as an integer (in cents)
- All styling is minimal and functional
- Built for speed and simplicity

---

Feel free to fork, adapt, and build on top of this for more advanced features like barcode scanning, real payment integration, etc.

Happy Hacking! 🚀
