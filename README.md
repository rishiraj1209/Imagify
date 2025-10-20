# Imagify — Text-to-Image SaaS Platform

[Live Demo](https://imagify-seven-cyan.vercel.app/)

## Overview
**Imagify** is a SaaS platform that converts text prompts into images using the **ClipDrop API**. It offers an easy-to-use interface with user authentication and a credit-based pricing model so users can generate AI images on demand.

## Features
- 🔐 **Authentication** — Signup / Login using JWT-based auth  
- 🖼 **Text → Image** — Generate images from text prompts via ClipDrop API  
- 💳 **Pricing & Credits** — Buy credits from the pricing panel to generate more images  
- 🎛️ **Responsive UI** — Built with React and Tailwind CSS  
- 🚀 **Deployed** — Frontend hosted on Vercel

## Tech Stack
- **Frontend:** React, Tailwind CSS  
- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (Mongoose)  
- **Auth:** JWT (JSON Web Tokens)  
- **API:** ClipDrop (Text-to-Image)  
- **Hosting:** Vercel (frontend), (suggested) Render/Heroku for backend

## Quick Start (Development)
```bash
# clone repo
git clone https://github.com/your-username/imagify.git
cd imagify
```

### Client
```bash
cd client
npm install
npm run dev
# opens at http://localhost:5173 (or the port Vite shows)
```

### Server
```bash
cd ../server
npm install
# create .env with required variables (see below)
npm run dev
# default server port depends on your setup (e.g. http://localhost:5000)
```

## Environment Variables (server/.env)
```env
MONGO_URI=your_mongodb_connection_string
CURRENCY =''
RAZORPAY_KEY_ID = '------------'
RAZORPAY_KEY_SECRET = '-------------'
CLIPDROP_API_KEY=your_clipdrop_api_key
FRONTEND_URL=http://localhost:5173
```

## Usage
1. Signup or Login.  
2. Use the text prompt box to describe the image you want.  
3. Generate an image — each generation consumes credits.  
4. Purchase credits from the Pricing panel to continue generating images.

## Deployment Notes
- Frontend can be deployed on Vercel.  
- Backend can be deployed on Render. 
- Set corresponding environment variables on your hosting provider.  
- For production, secure your API keys and enable HTTPS.


## Pricing Model (Example)
- **Free Tier** — Starter credits for new users.  
- **Paid Plans** — Different credit bundles (e.g., 100 credits / 500 credits).  
*(Implement payment gateway like Stripe or Razorpay for real transactions.)*

## Author
**Rishi Raj** — Computer Science and Data Analytics, IIT Patna

## Acknowledgements
- ClipDrop API — for text-to-image capability  
- Tailwind CSS — for UI styling
