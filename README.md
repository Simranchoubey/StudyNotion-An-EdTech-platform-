 # Studynotion Online Education Platform

 
**Live Demo**: {https://studynotion-edtech-project.vercel.app/}


![Main Page](images/mainpage.png)

## Project Description

Studynotion is a fully functional ed-tech platform that enables users to create, consume,
and rate educational content. The platform is built using the MERN stack, which includes
ReactJS, NodeJS, MongoDB, and ExpressJS.

Studynotion aims to provide:
- A seamless and interactive learning experience for students, making education
  more accessible and engaging.
- A platform for instructors to showcase their expertise and connect with learners
  across the globe.

In the following sections, we will cover the technical details of the platform, including:
1. System architecture: The high-level overview of the platform's components and
   diagrams of the architecture.
2. Front-end: The description of the front-end architecture, user interface design,
   features, and functionalities of the front-end, and frameworks, libraries, and tools
   used.
3. Back-end: The description of the back-end architecture, features and functionalities of
   the back-end, frameworks, libraries, tools used, and data models and database schema.
4. API Design: The description of the API design, list of API endpoints, their
   functionalities, and sample API requests and responses.
5. Deployment: The description of the deployment process, hosting environment and
   infrastructure, and deployment scripts and configuration.
6. Testing: The description of the testing process, types of testing, test frameworks and
   tools used.
7. Future Enhancements: The list of potential future enhancements to the platform,
   explanation of how these enhancements would improve the platform, estimated
   timeline and priority for implementing these enhancements.

In summary, Studynotion is a versatile and intuitive ed-tech platform that is designed to
provide an immersive learning experience to students and a platform for instructors to
showcase their expertise. In the following sections, we will delve into the technical details
of the platform, which will provide a comprehensive understanding of the platform's
features and functionalities.

## System Architecture

The Studynotion ed-tech platform consists of three main components: the front end, the
back end, and the database. The platform follows a client-server architecture, with the
front end serving as the client and the back end and database serving as the server.

### Front-end

The front end of the platform is built using ReactJS, which allows for the creation of dynamic and responsive user
interfaces, critical for providing an engaging learning experience to students.
The front end communicates with the back end using RESTful API calls.

### Back-end

The back end of the platform is built using NodeJS and ExpressJS. The back end
provides APIs for the front end to consume, which include functionalities such as user
authentication, course creation, and course consumption. The back end also handles the
logic for processing and storing the course content and user data.

### Database

The database for the platform is built using MongoDB, which is a NoSQL database that
provides a flexible and scalable data storage solution. MongoDB allows for the storage of
unstructured and semi-structured data. The database stores the course content, user data, and other
relevant information related to the platform.

![Architecture](images/architecture.png)

## Front End

The front end of Studynotion has all the necessary pages that an ed-tech platform should
have. Some of these pages include:

### For Students:
- Homepage: A brief introduction to the platform, with links to the course list and user details.
- Course List: A list of all the courses available on the platform, along with their descriptions and ratings.
- Wishlist: Displays courses that a student has added to their wishlist.
- Cart Checkout: Allows the user to complete course purchases.
- Course Content: Contains course materials, including videos and related resources.
- User Details: Displays account information such as name and email.
- User Edit Details: Allows students to edit their account details.

### For Instructors:
- Dashboard: Overview of the instructor's courses, ratings, and feedback.
- Insights: Detailed insights into course performance and engagement metrics.
- Course Management: Pages to create, update, and delete courses, and manage content and pricing.
- Profile Management: View and edit profile details.

To build the front end, we use frameworks and libraries such as ReactJS, Tailwind CSS, and other supportive tools.
To manage application state, Redux is used.

## Back End

Studynotion uses a monolithic architecture, with the backend built using Node.js, Express.js, and MongoDB as the primary database.

Features and Functionalities of the Back-end:
1. User authentication and authorization (including OTP verification and password reset).
2. Course management for instructors and course consumption for students.
3. Payment integration via Razorpay.
4. Cloud-based media management (Cloudinary) for storing media assets.
5. Markdown support for course content.

Frameworks, Libraries, and Tools used:
- Node.js
- MongoDB
- Express.js
- JWT for authentication
- Bcrypt for password hashing
- Mongoose for MongoDB object modeling

### Data Models and Database Schema:
- Student schema: name, email, password, and course details.
- Instructor schema: name, email, password, and course details.
- Course schema: course name, description, instructor details, and media content.

Overall, the back-end of Studynotion is designed to provide a robust and scalable solution for an ed-tech platform, focusing on security and reliability.

![Database Schema](images/schema.png)

## API Design

The Studynotion platform's API is designed following the REST architectural style. It uses JSON for data exchange and standard HTTP methods such as GET, POST, PUT, and DELETE.

Sample list of API endpoints and their functionalities:
1. /api/auth/signup (POST) - Create a new user (student or instructor) account.
2. /api/auth/login (POST) – Log in using existing credentials and generate a JWT token.
3. /api/auth/verify-otp (POST) - Verify the OTP sent to the user's registered email.
4. /api/auth/forgot-password (POST) - Send a password reset link to the registered email.
5. /api/courses (GET) - Get a list of all available courses.

In conclusion, the REST API design for the Studynotion ed-tech platform is a crucial part of the project, ensuring seamless communication between the front-end and back-end.

