# HoGo: Apartment Community Portal

A web portal for residents of an apartment complex, built on the MERN stack. Residents sign up,
talk to neighbours in one-to-one and group chats, pay the monthly maintenance bill online and
look up service contacts in a building directory.

## Features

- Sign-up and login with JWT authentication and hashed passwords
- Real-time one-to-one and group chat over Socket.IO, with new-message notifications
- Maintenance bill payment through Stripe Checkout (test mode)
- Directory of service contacts for the building

## Tech stack

- **Front end:** React, Chakra UI, React Router, Socket.IO client
- **Back end:** Node.js, Express, MongoDB with Mongoose, Socket.IO

## Running locally

You need Node.js and a MongoDB database (local or Atlas).

```bash
cd mern-chat-app-master
cp .env.example .env        # set MONGO_URI and JWT_SECRET
npm install
npm run server              # API on http://localhost:5000

cd frontend
npm install
npm start                   # UI on http://localhost:3000
```

## Team and credits

Group project with [@advaith017](https://github.com/advaith017), whose
[HoGo_Forum](https://github.com/advaith017/HoGo_Forum) repository this is forked from. I built
the maintenance payment page, the navigation between sections and the updated navbar and
styling. The chat forum is based on an open-source MERN chat app by Piyush Agarwal.
