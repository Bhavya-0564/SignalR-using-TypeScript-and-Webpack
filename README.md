# ⚡ SignalR with ASP.NET Core, TypeScript, and Webpack

A real-time web application demonstrating how to integrate **ASP.NET Core SignalR** with **TypeScript** and **Webpack** for dynamic two-way communication between client and server.

---

## 📌 Table of Contents

- [Features](#-features)  
- [Tech Stack](#-tech-stack)  
- [Project Structure](#-project-structure)  
- [How It Works](#-how-it-works)  

---

## 🚀 Features

- 🔄 Real-time messaging using SignalR  
- 🔧 Frontend built with TypeScript and bundled using Webpack  
- ⚙️ ASP.NET Core backend with SignalR Hub integration  
- 💬 Bi-directional communication between server and client  
- 📡 Live updates pushed without page refresh  

---

## 🧰 Tech Stack

- **Backend**: ASP.NET Core 9.0, SignalR  
- **Frontend**: TypeScript, Webpack, HTML, CSS  
- **Build Tools**: npm, Webpack, ts-loader  
- **IDE (Optional)**: Visual Studio 2022 / Visual Studio Code  

---

## 📁 Project Structure

SignalR-TypeScript-Webpack/
├── Controllers/
│ └── HomeController.cs # Serves the index page
├── Hubs/
│ └── ChatHub.cs # SignalR hub for real-time communication
├── ts/
│ └── main.ts # TypeScript client for SignalR
├── wwwroot/
│ ├── dist/
│ │ └── main.js # Webpack output (compiled from TypeScript)
│ └── index.html # Main UI page
├── package.json # npm dependencies
├── webpack.config.js # Webpack configuration
├── tsconfig.json # TypeScript configuration
├── Program.cs # Application entry point
└── SignalRApp.csproj # .NET Core project file


---

## 🔄 How It Works

1. The browser loads `index.html` and connects to the SignalR Hub defined in `ChatHub.cs`.  
2. TypeScript client code in `main.ts` establishes the connection using the SignalR JavaScript client.  
3. When a user sends a message:  
   - It is sent to the server-side `ChatHub`.  
   - The hub broadcasts the message to all connected clients.  
   - Clients receive and display the message instantly without reloading the page.

---


