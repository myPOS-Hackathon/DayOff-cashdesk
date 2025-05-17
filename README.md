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
secure-pos/
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

## Notes
- Total is sent as an integer (in cents)
- All styling is minimal and functional
- Built for speed and simplicity

---

Feel free to fork, adapt, and build on top of this for more advanced features like barcode scanning, real payment integration, etc.

Happy Hacking! 🚀
