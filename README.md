# Fast React Pizza 🍕

A modern pizza ordering web application built with React, showcasing advanced state management, routing, and styling practices. This project was designed as part of my transition from Vue to React, with a strong focus on app architecture, performance, and scalability. It demonstrates my ability to handle complex UI and remote states, manage asynchronous flows, and build user-centric experiences.

## 🚀 Features

- 🍕 Dynamic pizza menu fetched from an API
- 🛒 Add one or multiple pizzas to a cart before checkout
- 📍 Place orders with name, phone number, address, and optional GPS location
- ⚡ Mark orders as "priority" for an additional 20% fee, even after placing the order
- 📦 View your order by its unique ID
- ❌ No user login required, just input your name

## 🧱 Pages

- `/` : Homepage
- `/menu` : Pizza Menu
- `/cart` : View and manage cart items
- `/order/new` : Place a new order
- `/order/:orderId` : Look up a past order

## 🧠 State Management

| State | Type            | Managed With         |
| ----- | --------------- | -------------------- |
| User  | Global UI state | Redux                |
| Menu  | Remote data     | React Router Loaders |
| Cart  | Local UI state  | Redux                |
| Order | Remote data     | React Router + API   |

## 🛠 Technologies

- **React**
- **React Router v6.4+**
  > Used specifically in this project to explore its data APIs for remote state handling. In future projects, I plan to use **React Query**, which I find more scalable and better suited for real-world data fetching needs.
- **Redux Toolkit**
- **Tailwind CSS**
- **Vite**

## 🎯 Goals

- Practice advanced **React Router data APIs** (loaders, actions)
- Improve fluency in **Redux** for UI state
- Explore **clean architecture patterns** in a React SPA
- Showcase project structure, component modularity, and responsiveness
- Avoid using third-party payment APIs or login systems to stay focused on front-end architecture

## 📦 API Integration

- Pizza menu and order submission are handled through API calls (GET for menu, POST for new orders)
- Each order receives a unique ID to allow users to retrieve their order at any time
- Orders include user data + selected pizzas + optional priority flag
