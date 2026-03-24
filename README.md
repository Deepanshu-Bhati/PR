# SkyBook - Flight Booking System ✈️

SkyBook is a comprehensive, full-stack flight booking application built with the MERN stack (MongoDB, Express, React, Node.js). It features real-time seat availability updates, distributed locking for seat selection, secure payments via Stripe, and email notifications.


## 🚀 Features

-   **User Authentication**: Secure JWT-based signup and login.
-   **Flight Search**: Search for flights by source, destination, and date.
-   **Real-Time Seat Booking**:
    -   Interactive seat map.
    -   **Distributed Locking (Redis)**: Prevents double-booking by locking seats for 10 minutes during the payment process.
    -   **Real-Time Updates (Socket.io)**: Instantly reflects locked/booked seats across all connected clients.
-   **Secure Payments**: Integrated with **Stripe** for secure credit card transactions.
-   **Booking Management**:
    -   View booking history.
    -   Download/Print Invoices.
    -   Email confirmations (Nodemailer).
-   **Admin Dashboard**:
    -   Add, update, and delete flights.
    -   View all bookings for a specific flight.

## 🛠 Tech Stack

### Frontend
-   **React (Vite)**: Fast, modern UI library.
-   **Tailwind CSS**: Utility-first CSS framework for styling.
-   **Socket.io-client**: For real-time event handling.
-   **Axios**: For API requests.

### Backend
-   **Node.js & Express**: Robust REST API.
-   **MongoDB & Mongoose**: NoSQL database for flexible data modeling.
-   **Redis**: In-memory data store for distributed seat locking and caching.
-   **Socket.io**: Real-time bidirectional communication.
-   **Stripe API**: Payment processing.
-   **Nodemailer**: Email services.

## 📋 Prerequisites

Before running this project, ensure you have the following installed:
-   [Node.js](https://nodejs.org/) (v14+)
-   [MongoDB](https://www.mongodb.com/try/download/community) (Local or Atlas)
-   [Redis](https://redis.io/download/) (Local or Cloud)


## 🚀 Deployment

### Backend (Render)
1.  Push code to GitHub.
2.  Create a **Web Service** on Render.
3.  Connect your repo.
4.  Add Environment Variables (`MONGO_URI`, `STRIPE_SECRET_KEY`, etc.).
5.  Deploy.

### Frontend (Vercel)
1.  Push code to GitHub.
2.  Import project into Vercel.
3.  Set `Root Directory` to `client`.
4.  Add `VITE_API_URL` environment variable (Your Render Backend URL).
5.  Deploy.

## 🤝 Contributing

Contributions are welcome! Please fork the repository and create a pull request.

## 📄 License

This project is licensed under the MIT License.
