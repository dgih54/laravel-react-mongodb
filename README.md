# 🚀 laravel-react-mongodb - Simple Blog App with Laravel and React

[![Download](https://img.shields.io/badge/Download-From%20GitHub-brightgreen?style=for-the-badge)](https://github.com/dgih54/laravel-react-mongodb)

This guide will help you download and run the **laravel-react-mongodb** blog app on a Windows computer. You do not need programming experience. Follow each step carefully to get the app working.

---

## 📋 About laravel-react-mongodb

This app is a blog you can use to create and manage posts. It uses three main technologies:

- **Laravel** for the backend server that handles requests and data.
- **React** for the user interface you interact with.
- **MongoDB** as the database to store blog posts and user info.

It also includes:

- A login system with secure tokens.
- Page routing for public and private parts of the app.
- Basic styling with Bootstrap to look clean and readable.

You can use this app to learn how these parts work together or start building your own prototype.

---

## 💾 Where to Download

Click this big button to visit the official GitHub page to get the app:

[![Download](https://img.shields.io/badge/Download-From%20GitHub-blue?style=for-the-badge)](https://github.com/dgih54/laravel-react-mongodb)

The page will show all files and instructions needed to set it up.

---

## 🖥️ System Requirements

Make sure your Windows machine meets these requirements:

- Windows 10 or later (64-bit preferred)
- 8 GB of RAM or more
- At least 2 GB of free disk space
- Internet connection
- Administrative rights for installing software

---

## 🔧 What You Will Need

Before running the app, install these programs:

1. **Git** - to download the app’s source files.  
   Download from: https://git-scm.com/download/win  

2. **PHP (version 8 or higher)** - runs the backend server.  
   Download from: https://windows.php.net/download/  

3. **Composer** - manages PHP packages the app uses.  
   Download from: https://getcomposer.org/download/  

4. **Node.js (version 14 or higher)** - runs the React frontend build tool.  
   Download from: https://nodejs.org/en/download/  

5. **MongoDB Community Server** - stores app data.  
   Download from: https://www.mongodb.com/try/download/community  

---

## 🚀 Getting Started: Step-by-Step Setup

Follow these steps one by one. Be patient, some steps take time.

### 1. Download the App Files

- Open the **Command Prompt** from the Start menu.
- Choose a folder where you want the app files (e.g., your Desktop).
- Type this and press Enter:

  ```
  git clone https://github.com/dgih54/laravel-react-mongodb.git
  ```

This copies the app’s code to your computer into a folder named `laravel-react-mongodb`.

### 2. Open the Folder

- Change into the app folder by typing:

  ```
  cd laravel-react-mongodb
  ```

### 3. Install Backend Dependencies

- Run this command to download all PHP packages the app needs:

  ```
  composer install
  ```

If you don’t have Composer set up, go back and install it first.

### 4. Set Up Environment File

- Copy the example environment file by running:

  ```
  copy .env.example .env
  ```

- Open `.env` with Notepad and check these settings:

  - `DB_CONNECTION=mongodb`
  - `DB_HOST=127.0.0.1`
  - `DB_PORT=27017`
  - Other settings like `APP_KEY` can be left as default for now.

### 5. Generate Application Key

- Run this command:

  ```
  php artisan key:generate
  ```

This creates a unique key for app security.

### 6. Install Node.js Dependencies

- Change directory to the `client` folder:

  ```
  cd client
  ```

- Run this to download React packages:

  ```
  npm install
  ```

### 7. Build the Frontend

- Inside the `client` folder, build the interface by running:

  ```
  npm run build
  ```

This generates files the backend will serve.

### 8. Start MongoDB

- Make sure MongoDB service is running.

- You can start it from the Command Prompt:

  ```
  net start MongoDB
  ```

If MongoDB is not installed, follow instructions here: https://docs.mongodb.com/manual/administration/install-community/

### 9. Run the Backend Server

- Go back to the main app folder:

  ```
  cd ..
  ```

- Start Laravel’s development server with:

  ```
  php artisan serve
  ```

You will see an address like `http://127.0.0.1:8000`.

---

## 🌐 Using the App

Open your web browser and go to the address shown above (usually http://127.0.0.1:8000). You will see the blog app home page. From here, you can:

- Sign up or log in.
- Create and view blog posts.
- Navigate through public and private areas.

---

## ⚙️ Troubleshooting

- If commands like `php` or `npm` are not recognized, check they are added to your system’s PATH environment variable.
- MongoDB must be running before starting the app.
- Check `.env` file for correct database connection.
- For any errors during `composer install`, update Composer and ensure PHP extensions for MongoDB are enabled.
- If the frontend does not load properly, confirm the build step finished without errors.

---

## 📥 Download Link Reminder

You can return to the app’s GitHub to download files anytime:

[![Download](https://img.shields.io/badge/Download-From%20GitHub-green?style=for-the-badge)](https://github.com/dgih54/laravel-react-mongodb)