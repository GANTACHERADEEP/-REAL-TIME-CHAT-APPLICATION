# REAL-TIME-CHAT APPLICATION

*COMPANY NAME* : CODTECH IT SOLUTIONS PVT.LTD

*NAME* : GANTA CHERADEEP

*INTERN ID* : CT04DF694

*DOMAIN NAME* : FRONTEND WEB DEVELOPMENT

*DURATION* : 4-WEEKS

*MENTOR NAME* : NEELA SANTHOSH

## Project Description:  Real-Time Chat Application using WebSockets and React

As part of my learning and internship task, I worked on building a Real-Time Chat Application using WebSockets and React. The objective of this mini-project was to implement a real-time communication system where multiple users can chat simultaneously with instant message updates, without needing to refresh the page. The overall project helped me understand full-stack development, how client-server communication works in real time, and how to integrate different technologies efficiently.

I used Visual Studio Code (VS Code) as my primary code editor throughout the project. It provided a smooth development experience with built-in terminal support, Git integration, and extensions like Prettier, ESLint, and React snippets which helped in speeding up the coding process.

##Project Setup & Directory Structure
To begin, I created two separate directories for the client and server:

bash

mkdir realtime-chat
cd realtime-chat
mkdir client
mkdir server

The client folder contains the React frontend, and the server folder holds the Node.js backend. I used the following commands to initialize each side:

For the server:
bash

cd server
npm init -y
npm install express ws

Here, I used express for setting up a basic HTTP server and ws, a lightweight and simple WebSocket implementation for Node.js. The ws package allows full control over WebSocket connections, message broadcasting, and client management.

I wrote the WebSocket server logic such that when a client connects, it listens for messages. Whenever a message is received from any user, it is broadcast to all connected clients.

 ##Backend (WebSocket) Logic you can see in the file provided
## React Frontend Setup
For the frontend, I navigated into the client folder and ran:

bash

npx create-react-app .
This bootstrapped a full React application. I then implemented a simple chat interface with an input field and a message list. WebSocket connection was handled using useEffect, and messages were managed using useState.

The frontend connects to the backend WebSocket server using:

const socket = new WebSocket('ws://localhost:3001');

Messages sent via this socket are displayed instantly in the chat window, and any new messages from other users are also rendered live.

Initially, I faced issues understanding how WebSockets maintain persistent connections, unlike HTTP. After reading official documentation and watching video tutorials, I understood that WebSockets are ideal for real-time apps like chat, gaming, and live dashboards because they enable two-way communication over a single TCP connection.

Using the ws library gave me exposure to working directly with the WebSocket protocol rather than relying on abstractions like Socket.IO. This helped me better understand message handling, broadcasting, and how clients are managed at the server level.

Additionally, I practiced using various VS Code features, such as the integrated terminal, auto-formatting, debugging, and version control with Git. These helped streamline the development workflow.

##Conclusion
This project was a hands-on introduction to building real-time web applications. I successfully created a simple, working real-time chat application using React and WebSockets. I understood the importance of managing state in React, persistent server-client communication, and the significance of libraries like ws and express in building scalable backend services. Future enhancements can include message timestamps, user authentication, MongoDB integration for storing chat history, and deploying the app on cloud platforms like Vercel and Render.

#output :




