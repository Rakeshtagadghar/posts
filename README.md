# NextPosts - A Simple Social Media Feed

This is a simple social media feed application built with Next.js. It allows users to create posts with images and like or unlike posts from other users. The project demonstrates modern Next.js features, including Server Actions, optimistic UI updates, and data handling with a local SQLite database.

## Features

-   Create new posts with a title, content, and an image.
-   View a feed of all posts.
-   Like and unlike posts.
-   Optimistic UI updates for a fast and responsive user experience when liking posts.
-   Image uploads are handled by Cloudinary.

## Prerequisites

Before you begin, ensure you have the following installed on your local machine:

-   [Node.js](https://nodejs.org/en) (v18 or later recommended)
-   [npm](https://www.npmjs.com/) (comes with Node.js)

## Getting Started

Follow these steps to get the project up and running on your local machine.

### 1. Install Dependencies

First, navigate to the project directory and install the required dependencies using npm:

```bash
npm install
```

### 2. Configure Environment Variables

This project uses Cloudinary to handle image uploads. You will need to create an account with [Cloudinary](https://cloudinary.com/) to get the necessary credentials.

Once you have your credentials, create a file named `.env.local` in the root of the project directory and add the following environment variables:

```.env.local
CLOUDINARY_CLOUD_NAME="your-cloud-name"
CLOUDINARY_API_KEY="your-api-key"
CLOUDINARY_API_SECRET="your-api-secret"
```

Replace `"your-cloud-name"`, `"your-api-key"`, and `"your-api-secret"` with your actual Cloudinary credentials.

**Note:** The application will not be able to upload images without these variables.

### 3. Running the Application

Once the dependencies are installed and the environment variables are configured, you can start the development server:

```bash
npm run dev
```

The application will start, and a local SQLite database file (`posts.db`) will be created automatically with the necessary tables and dummy data.

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application in action.

## Available Scripts

In the project directory, you can run the following scripts:

-   `npm run dev`: Runs the app in development mode.
-   `npm run build`: Builds the app for production.
-   `npm run start`: Starts a production server.
-   `npm run lint`: Runs the Next.js linter. 