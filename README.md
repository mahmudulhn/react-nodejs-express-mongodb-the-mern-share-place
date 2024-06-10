# Share Place Project Documentation

## Project Structure

The project is divided into two main directories: `backend` and `react-frontend`.

### Backend

The backend directory contains the server-side code, built with Node.js, Express.js, and MongoDB. Here's a detailed breakdown of its structure:

- **Root Files**

  - `.gitignore`: Specifies files to be ignored by Git.
  - `app.js`: Main application file where the Express server is configured and routes are set up.
  - `nodemon.json`: Configuration file for nodemon to automatically restart the server on file changes.
  - `package.json`: Lists the dependencies and scripts for the backend project.
  - `package-lock.json`: Locks the versions of installed dependencies.

- **Controllers**

  - `places-controllers.js`: Handles the logic for place-related routes.
  - `users-controllers.js`: Handles the logic for user-related routes.

- **Middleware**

  - `check-auth.js`: Middleware to check user authentication.
  - `file-upload.js`: Middleware for handling file uploads.

- **Models**

  - `http-error.js`: Custom error model.
  - `place.js`: Mongoose schema and model for places.
  - `user.js`: Mongoose schema and model for users.

- **Routes**

  - `places-routes.js`: Route definitions for place-related endpoints.
  - `users-routes.js`: Route definitions for user-related endpoints.

- **Uploads**

  - Contains uploaded images.

- **Util**
  - `location.js`: Utility functions related to location handling.

### React Frontend

The frontend directory contains the client-side code, built with React. Here's a detailed breakdown of its structure:

- **Root Files**

  - `.env`: Environment variables.
  - `.gitignore`: Specifies files to be ignored by Git.
  - `package.json`: Lists the dependencies and scripts for the frontend project.
  - `package-lock.json`: Locks the versions of installed dependencies.

- **Build**

  - Contains the production build of the React application.

- **Public**

  - Static files like `index.html` and images.

- **Src**

  - Main source directory for the React application.

  - **Assets**

    - Contains images and CSS files.

  - **Components**

    - **FormElements**: Components related to form handling.
      - `Button.js`: Custom button component.
      - `ImageUpload.js`: Component for image upload functionality.
      - `Input.js`: Custom input component.
    - **Navigation**: Components related to navigation.
      - `MainHeader.js`: Main header component.
      - `MainNavigation.js`: Main navigation bar component.
      - `NavLinks.js`: Navigation links component.
      - `SideDrawer.js`: Side drawer component for mobile view.
    - **UIElements**: Common UI components.
      - `Avatar.js`: Avatar component.
      - `Backdrop.js`: Backdrop component for modals.
      - `Card.js`: Card component.
      - `ErrorModal.js`: Error modal component.
      - `LoadingSpinner.js`: Loading spinner component.
      - `Map.js`: Map component.
      - `Modal.js`: Modal component.

  - **Context**

    - `auth-context.js`: Context for authentication state.

  - **Hooks**

    - `auth-hook.js`: Custom hook for handling authentication.
    - `form-hook.js`: Custom hook for form management.
    - `http-hook.js`: Custom hook for HTTP requests.

  - **Util**

    - `validators.js`: Utility functions for form validation.

  - **User Components**

    - `UserItem.js`: Component for rendering individual user items.
    - `UsersList.js`: Component for rendering a list of users.

  - **User Pages**
    - `Auth.js`: Authentication page component.
    - `Users.js`: Users listing page component.

## Setup and Installation

1. **Backend Setup**

   - Navigate to the `backend` directory.
   - Run `npm install` to install dependencies.
   - Start the server using `npm start` or `nodemon app.js`.

2. **Frontend Setup**
   - Navigate to the `react-frontend` directory.
   - Run `npm install` to install dependencies.
   - Start the development server using `npm start`.

## Key Functionalities

- **Authentication**: User registration and login with JWT-based authentication.
- **Places Management**: Users can create, read, update, and delete places.
- **File Uploads**: Handling image uploads for user profiles and places.
- **Real-Time Updates**: Responsive design with real-time updates using React hooks and context.

## Conclusion

This MERN stack project provides a comprehensive guide to building a full-stack application with user authentication, CRUD operations, and image uploads. The structured directory and modular components make it easy to maintain and extend.
