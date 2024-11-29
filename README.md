# 3MTT FINAL CAPSTONE PROJECT.

## Project Title: `TaskMaster`

# PROJECT DIFINITION:
- Set reminders, and categorize tasks based on urgency and importance. 
- With functionalities such as due dates, recurring tasks, and progress tracking, `TastMaster` aims to enhance productivity and streamline the planning process for personal and professional tasks.


| AIM | PURPOSE |
| ------ | ------ |
| The primary aim of `TaskMaster` is to empower users to take control of their time and responsibilities by providing them with a comprehensive tool for task management. This application seeks to: |The purpose of `TaskMaster` is to address the common challenges individuals face in managing their daily tasks and responsibilities. By offering a user-friendly platform, the project aims to:|
|0. Facilitate effective organization of tasks and commitments. |Reduce overwhelm and stress associated with task management by providing clear visibility of priorities and deadlines.|
|1. Enhance user productivity by promoting better time management and prioritization.|Encourage users to set and achieve personal and professional goals through structured planning.|
|2. Foster a sense of accomplishment through progress tracking and completion of tasks. |Support a balanced lifestyle by allowing users to integrate both work and personal tasks seamlessly.|


#Technology Used:
- HTML
- CSS
- JAVASCRIPT
- ReactJs
- NodeJs
- ExpressJs

#DateBase Used:
- MongoDB


# Task Master Monorepo

This monorepo contains a **Vite React client** and an **Express server** for building and serving a full-stack web application.

## Table of Contents

- [Structure](#structure)
- [Requirements](#requirements)
- [Setup](#setup)
- [Scripts](#scripts)
- [Development](#development)
- [Build](#build)
- [Proxy Configuration](#proxy-configuration)
- [Production Deployment](#production-deployment)

---

## Structure

taskMaster/ 
├── client/ # Vite React application 
├── server/ # Express API server 
├── package.json # Root package.json with scripts and dependencies

## Requirements

- Node.js v16 or higher
- npm v7 or higher

---

## Setup

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd task-nest

2. Install dependencies for the root, client, and server:
   ```
npm install
npm install --prefix client
npm install --prefix server
   ```

3. Ensure your server is running on http://localhost:5000


Scripts
Root Scripts

Start Both Client and Server:
npm run dev

Start Server Only:
npm run dev:server

Start Client Only:
npm run dev:client

Build Both Client and Server:
npm run build

Client-Specific Scripts

Start Development Server:
npm run dev --prefix client

Build Production Client:
npm run build --prefix client

Preview Production Build:
npm run preview --prefix client

Server-Specific Scripts

Start Development Server:
npm run dev --prefix server

Start Production Server:
npm run start --prefix server

Build Server (if applicable):
npm run build --prefix server

Development
To start the development environment for both the client and server simultaneously, run:

npm run dev

This will:

Start the Express server on http://localhost:5000.
Start the Vite development server on http://localhost:3000.


Build
To build both the client and server, run:

npm run build

This will:

Build the client into the client/dist folder.
Prepare the server for production deployment.


Production Deployment

For Client
Serve the client/dist folder using a static file server (e.g., Nginx).

For Server
Run the built server using Node.js:

node server/index.js


Combined Deployment
Use a reverse proxy (like Nginx) to serve both the client and API from a single domain.