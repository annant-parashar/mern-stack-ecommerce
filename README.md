# MERN Stack E-Commerce

A complete, full-stack E-Commerce application built using the MERN stack (MongoDB, Express.js, React.js, Node.js). This project is divided into three main components: a customer-facing frontend, an admin dashboard, and a robust backend API.

##  Features

###  Frontend
- Modern, responsive user interface built with **React 19** and **Tailwind CSS**.
- Lightning-fast development and build times powered by **Vite**.
- Seamless client-side routing via **React Router v7**.
- User-friendly notifications using **React Hot Toast** and **React Toastify**.
- Asynchronous API requests with **Axios**.

###  Admin Dashboard
- Secure management portal for store owners.
- Built with **React 19**, **Vite**, and **Tailwind CSS**.
- Manage products, view customer orders, and control inventory.

###  Backend API
- RESTful API built with **Node.js** and **Express.js** using ES Modules.
- Data modeling and database interaction using **MongoDB** and **Mongoose**.
- Secure authentication system using **JSON Web Tokens (JWT)** and **bcrypt**.
- Integrated media management for product images using **Cloudinary** and **Multer**.
- Dual payment gateway integration supporting both **Stripe** and **Razorpay**.

##  Project Structure

```text
mern-stack-ecommerce/
├── admin/       # React application for store management
├── backend/     # Node.js/Express API server
└── frontend/    # React application for the customer storefront
```

##  Getting Started

### Prerequisites
Make sure you have the following installed on your machine:
- Node.js (v18 or higher recommended)
- npm or yarn
- MongoDB (local or MongoDB Atlas)
- Cloudinary Account (for image uploads)
- Stripe / Razorpay Accounts (for payments)

### Installation

Clone the repository and install the dependencies for each part of the project.

**1. Clone the repository:**
```bash
git clone https://github.com/annant-parashar/mern-stack-ecommerce.git
cd mern-stack-ecommerce
```

**2. Install Backend Dependencies:**
```bash
cd backend
npm install
```

**3. Install Frontend Dependencies:**
```bash
cd ../frontend
npm install
```

**4. Install Admin Dependencies:**
```bash
cd ../admin
npm install
```

### Environment Variables

You need to set up environment variables for the **backend**. Create a `.env` file in the `/backend` directory and add the following keys (replace with your actual credentials):

```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key

# Cloudinary Setup
CLOUDINARY_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_api_secret

# Payment Gateways (Depending on what you use)
STRIPE_SECRET_KEY=your_stripe_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

### Running the Application

You will need three separate terminal windows to run the frontend, admin, and backend concurrently.

**Start the Backend Server:**
```bash
cd backend
npm run server
```
*The API will be running on http://localhost:4000*

**Start the Frontend:**
```bash
cd frontend
npm run dev
```

**Start the Admin Dashboard:**
```bash
cd admin
npm run dev
```

##  Deployment
The project contains `vercel.json` configuration files in each directory, making it ready for seamless deployment on platforms like [Vercel](https://vercel.com).
