
# QuickChat - Real-Time Chat Application

**QuickChat** is a full-stack web application designed for real-time communication between users. This chat application allows users to send text and media messages, manage their profiles, and chat with multiple users in an interactive and responsive interface. The app is built using modern web technologies, ensuring scalability, security, and a great user experience.

## Key Features

- **Real-Time Messaging**: Chat with users instantly, supporting both text and media messages.
- **User Authentication**: Secure user registration, login, and profile management.
- **Profile Management**: Users can update their profiles, including profile pictures and bios.
- **Media Sharing**: Ability to send images as part of the chat.
- **Responsive Design**: Fully responsive for both desktop and mobile devices.
- **Real-Time Updates**: Display online/offline status and unread messages in real-time.

## Technologies Used

- **Frontend**: 
  - React.js
  - HTML5 / CSS3
  - React Hooks, Context API
- **Backend**:
  - Node.js with Express.js
  - MongoDB (via Mongoose)
  - JWT (JSON Web Tokens) for authentication
  - Cloudinary for image/file uploads
- **Other**:
  - Bcrypt.js for password hashing
  - React-Hot-Toast for notifications
  - WebSockets for real-time communication (optional based on your implementation)
- **Deployment**:
  - Frontend: Vercel
  - Backend: Heroku (or another cloud service)
  - MongoDB: MongoDB Atlas

## Installation Instructions

### Prerequisites

Before running the project, make sure you have the following installed:

- **Node.js**: [Download Node.js](https://nodejs.org/)
- **MongoDB Atlas**: Set up an account and create a MongoDB cluster [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
- **Cloudinary**: Sign up for a Cloudinary account [Cloudinary](https://cloudinary.com/)

### Setup Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/Kush146/Quickchat-Fullstack.git
   ```

2. Change into the project directory:

   ```bash
   cd Quickchat-Fullstack
   ```

3. Install the necessary dependencies for both frontend and backend:

   - **Frontend** (React):

     Navigate to the `frontend` folder (if it's in a sub-folder) and install the dependencies:
     ```bash
     cd frontend
     npm install
     ```

   - **Backend** (Node.js):

     Navigate to the `backend` folder (if it's in a sub-folder) and install the dependencies:
     ```bash
     cd backend
     npm install
     ```

4. Create a `.env` file in both the **frontend** and **backend** directories with the necessary environment variables, including:
   - **MongoDB URI** for your MongoDB database
   - **Cloudinary API credentials** (cloud name, API key, secret)
   - **JWT Secret** for authentication

   Example `.env` for the backend:

   ```
   MONGO_URI=your_mongo_uri
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

5. **Start the Development Server**:

   For the backend:
   ```bash
   npm start
   ```

   For the frontend:
   ```bash
   npm start
   ```

6. Your app should now be running locally. Open your browser and visit `http://localhost:3000` (or the relevant port for your setup).

### Deployment

To deploy the application:

1. **Frontend Deployment**:
   - You can deploy the frontend to Vercel by following their [documentation](https://vercel.com/docs).

2. **Backend Deployment**:
   - The backend can be deployed to platforms like **Heroku**, **DigitalOcean**, or **AWS**. For Heroku:
     ```bash
     heroku create
     git push heroku main
     ```

   - Ensure that you set the environment variables on your deployment platform (Heroku, etc.) to match your `.env` file.

---

## Contribution Guidelines

If you'd like to contribute to QuickChat, follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a pull request.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
