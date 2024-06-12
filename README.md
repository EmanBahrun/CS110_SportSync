# SportSync

SportSync is an online platform for organizing, sharing, and creating local sporting events specifically for UCR students. This project aims to foster community engagement, promote physical activity, and simplify the process of finding and joining sports events on campus.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [License](#license)
- [Task Allocation](#task-allocation)

## Introduction

SportSync is designed to make it easy for UCR students to connect with each other through sports. Whether you're looking to join a casual pick-up game or organize a tournament, SportSync has you covered. Our platform provides a seamless way to create, discover, and participate in sporting events tailored to the UCR community.

## Features

- **Event Creation**: Easily create sports events with details like date, time, location, and participant limit.
- **Event Discovery**: Browse and join upcoming sports events on campus.
- **User Profiles**: Manage your profile, track your participation history, and connect with other users.
- **Notifications**: Receive updates about upcoming events and reminders for events you've joined.
- **Ratings and Comments**: Rate events and leave feedback to help improve future events.

## Installation

To get started with SportSync, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/EmanBahrun/SportSync4.git
    cd SportSync4 
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    ```

3. **Set Up Environment Variables**:
    Create a `.env` file in the root directory and add the following variables:
    ```bash

    STRIPE_WEBHOOK_SECRET=
    NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
    STRIPE_SECRET_KEY=

    NEXTPUBLIC_SERVER_URL=http://localhost:3000/

    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    WEBHOOK_SECRET=

    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

    MONGODB_URI=

    UPLOADTHING_SECRET=
    UPLOADTHING_APP_ID=
    ```

4. **Start the Server**:
    ```bash
    npm start
    ```

5. **Navigate to the Application**:
    Open your browser and go to `http://localhost:3000`.

## Usage

1. **Sign Up**: Create a new account using your UCR email.
2. **Create an Event**: Click on "Create Event" and fill out the event details.
3. **Join an Event**: Browse the list of upcoming events and click "Join" to participate.
4. **Manage Profile**: Update your profile with your interests and track your event history.

## Technologies Used

- **Frontend**: Next.js, React, TypeScript, TailwindCSS
- **Backend**: Node.js
- **Database**: MongoDB
- **Authentication**: Clerk
- **Payment Processing**: Stripe
- **Validation**: Zod
-

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Task Allocation

- **Frontend Development**: 
    - **Eman Bahrun**: Developed the user interface using Next.js and React, ensuring a responsive and user-friendly design with TailwindCSS.
    - **David Jordan**: Implemented dynamic components and managed the integration of frontend libraries such as React Hook Form.

- **Backend Development**:
    - **Hung Pham**: Handled authentication and API development using Node.js. Focused on event management and implemented robust security measures, integrating Clerk for authentication and Stripe for payment processing.

- **Database Management**: 
    - **Matu Kahsay**: Designed and maintained the MongoDB database schema. Managed data interactions and ensured efficient and secure data storage and retrieval.

- **Testing and Deployment**: 
    - **All Members**: Collaboratively tested the application for functionality, performance, and security. Managed the deployment process on Heroku, ensuring a smooth and reliable release of the application.
