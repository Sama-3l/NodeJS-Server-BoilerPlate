# Node.js Backend Boilerplate

This repository provides a production-ready boilerplate for a Node.js backend server. It includes environment-specific configurations, error logging, and middleware support. This structure helps you quickly set up a robust and scalable server for production-level applications.

## Features

- **Environment Switching**: Use `NODE_ENV` to switch between development and production configurations.
- **Error Handling**: Built-in error handling middleware to capture, log, and manage errors gracefully.
- **Custom Scripts**: Includes `start:dev` and `start:prod` commands for easy environment-specific server startup.
- **Logging**: Ready-to-use error logging utility.

## Table of Contents

- [Installation](#installation)
- [Project Structure](#project-structure)
- [Scripts](#scripts)
- [Environment Variables](#environment-variables)
- [Error Handling](#error-handling)
- [Running the Server](#running-the-server)
- [License](#license)

---

## Installation

Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/yourusername/nodejs-backend-boilerplate.git
cd nodejs-backend-boilerplate
npm install
```

## Project Structure

```bash
├── server.js               # Main entry point
├── package.json            # NPM configuration and scripts
├── /config                 # Environment-specific configuration files
│   ├── .env                # Default environment variables (production)
│   ├── .env.dev            # Development environment variables
├── /utils
│   └── error-handler.js    # Custom error handling middleware
├── /logs                   # Error log storage
└── /src                    # Main application logic
    ├── /routes             # API routes
    ├── /controllers        # Request handlers
    └── /models             # Database models
```

## Scripts

Here are the available scripts for different environments:

- **Start Development Server**: Runs the server with NODE_ENV=development.