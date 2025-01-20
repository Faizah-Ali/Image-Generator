# Image Generation App 

Welcome to the Image Generation App! This app allows users to generate custom images based on specific input parameters or prompts. Built using the MERN stack along with SQL for structured data storage, the app provides a seamless and interactive user experience for image generation.

## Overview

The application allows users to input criteria such as style, size, or other attributes to generate personalized images. It features an easy-to-use interface, responsive design, real-time feedback, and an optimized backend that handles user requests efficiently.

---

## Table of Contents

- [Technologies Used](#technologies-used)
- [Features](#features)
- [Installation Instructions](#installation-instructions)
  - [Server-side Setup](#server-side-setup)
  - [Client-side Setup](#client-side-setup)
- [Environment Variables](#environment-variables)
- [Running the Application](#running-the-application)
- [Contributing](#contributing)
- [License](#license)

---

## Technologies Used

- **Frontend**: React.js, Axios, MUI (Material UI), Styled Components, React Router
- **Backend**: Node.js, Express.js, Cloudinary (for image management), OpenAI API
- **Database**: SQL (for structured data storage and management)
- **Deployment**: Heroku (for cloud hosting)

---

## Features

- **Image Generation**: Users can input various parameters (style, size, etc.) to generate customized images based on specific criteria.
- **Responsive UI**: The app's interface adapts to different devices, providing a smooth user experience on both mobile and desktop.
- **Real-time Feedback**: As users enter input, the app processes requests and displays generated images instantly.
- **User Authentication (optional)**: Allows users to create accounts, track their image generation history, and manage their profiles.
- **Admin Panel**: Restaurant or platform administrators can manage and view the image generation data and analytics.

---

## Installation Instructions

### Server-side Setup

To set up the server, you’ll need to install the necessary dependencies in the server folder.

1. Clone the repository:

    ```bash
    git clone https://github.com/Faizah-Ali/Image-Generator.git
    cd Image-Generator
    ```

2. Install server-side dependencies:

    Navigate to the `server` folder and run:

    ```bash
    npm install cloudinary cors dotenv express mongoose nodemon openai
    ```

3. Set up the necessary environment variables in a `.env` file. Here’s an example of what it should look like:

    ```
    CLOUDINARY_CLOUD_NAME=<your-cloud-name>
    CLOUDINARY_API_KEY=<your-api-key>
    CLOUDINARY_API_SECRET=<your-api-secret>
    OPENAI_API_KEY=<your-openai-api-key>
    PORT=5000
    ```

4. Run the server:

    ```bash
    npm run dev
    ```

   This will start the backend server on the specified port (default: 5000).

### Client-side Setup

To set up the client, you’ll need to install the required dependencies in the `client` folder.

1. Navigate to the `client` folder and install the client-side libraries:

    ```bash
    cd client
    npm install @emotion/react @emotion/styled @mui/icons-material @mui/lab @mui/material axios file-saver react-lazy-load-image-component react-router-dom styled-components
    ```

2. After installation, you can start the client-side application:

    ```bash
    npm start
    ```

   This will start the React app, which should now be running on [http://localhost:3000](http://localhost:3000).

---

## Environment Variables

Here are the environment variables you need for both the client and server to work correctly:

### Server-side:
- `CLOUDINARY_CLOUD_NAME`: Cloudinary cloud name (for image storage).
- `CLOUDINARY_API_KEY`: Cloudinary API key.
- `CLOUDINARY_API_SECRET`: Cloudinary API secret.
- `OPENAI_API_KEY`: OpenAI API key (for generating custom images).
- `PORT`: Port number to run the server (default is `5000`).

### Client-side:
The client-side application does not require any additional environment variables at the moment.

---

## Running the Application

After following the installation instructions for both the server and client, you can run the full-stack app locally. 

1. **Backend**: 
   - Navigate to the `server` directory and start the server by running:

     ```bash
     npm run dev
     ```

   - This will run the backend on `http://localhost:5000`.

2. **Frontend**: 
   - Navigate to the `client` directory and start the React app by running:

     ```bash
     npm start
     ```

   - This will run the frontend on `http://localhost:3000`.

Both should work together, and you can now generate custom images by interacting with the frontend.

---

## Contributing

We welcome contributions to improve this app! If you want to contribute, follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a pull request.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
