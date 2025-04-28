# Phase 4 – Project Presentation

> [!NOTE]  
> Think of this as presenting your project, which you can include in your job application. The presentation should be clear and concise. Explain the entire project. Don't be afraid to highlight failures, as everyone has experienced them at some point. Consider that the viewer may not have a strong technical background.  
>   
> **You can do this entire presentation in English or Finnish.**

## 🎯 Project title
Personal Learning Tracker (PLT): A Comprehensive Tool for Managing Courses and Assignments
This title reflects the application's purpose of helping students efficiently manage their educational activities across various platforms and institutions.

---

## 📝 Project overview

The Personal Learning Tracker (PLT) is a web-based application designed to assist students in managing and tracking their courses, assignments, and class schedules from multiple universities and online platforms. In Finland, where students can enroll in courses from various institutions such as MOOC.FI, FITECH, EDX, and Coursera, it can be challenging to keep track of all course schedules and assignment deadlines in one place.
The PLT provides a centralized platform where students can input, view, and manage all course-related activities efficiently. By offering features such as course management, assignment tracking, and a visual calendar, the application aims to enhance students' organizational skills, improve time management, and ultimately support their academic success.
The target users include exchange students, local university students, and part-time learners who juggle multiple courses and responsibilities. The PLT is designed to simplify their educational experience, making it easier to stay on top of deadlines and manage their learning journey effectively.

---

## 📌 Use case summary

_Link to the use cases defined in Phase 1._
[Original Use Cases](https://github.com/supaizjy0321/PersonalLearningTracker/blob/main/1_Definition_and_Planning.md#2-use-cases-and-usage-scenarios)


| Original Use Case | Implemented (Yes/No) | Demonstration / Notes |
|----------|----------------------|------------------------|
| Adding a New Course | Yes | Implemented with a user-friendly form for course details. Demonstration will be shown live. |
| Adding an Assignment Deadline | Yes | Integrated with the calendar view to display deadlines. Demonstration will be shown live. |
| Viewing the Calendar | Yes | Enhanced with visual indicators for assignment status. Demonstration will be shown live. |
| Editing Course Information | Yes | Allows updates to course details through an intuitive interface. Demonstration will be shown live. |
| Tracking Study Hours | Yes | Incremental tracking with immediate visual feedback. Demonstration will be shown live. |

| Extra Use Case | Implemented (Yes/No) | Demonstration / Notes |
|----------|----------------------|------------------------|
| Deleting an Assignment | Yes | Removes assignment from both the course view and the calendar. Demonstration will be shown live. |
| Deleting a Course | Yes | Deletes course and all associated assignments from the system. Demonstration will be shown live. |
| Accessing Course Materials | Yes | Opens course links in new tabs for easy access. Demonstration will be shown live. |
| Minimizing/Maximizing Courses | Yes | Improves interface organization by allowing users to collapse course details. Demonstration will be shown live. |

---
## ✍️ Technical implementation

### Technologies Used

#### Frontend:
- **React**: A JavaScript library for building user interfaces, allowing for the creation of dynamic and responsive web applications.
- **React Router**: Used for client-side routing, enabling seamless navigation between different pages without full page reloads.
- **CSS**: Custom stylesheets for visual design, ensuring a clean and user-friendly interface.

#### Backend:
- **Node.js**: A JavaScript runtime for building scalable server-side applications.
- **Express**: A web application framework for Node.js that simplifies the creation of RESTful APIs.
- **PostgreSQL**: A powerful relational database used for storing course and assignment data, hosted on Azure for reliability and scalability.

#### Cloud Services:
- **Azure App Service**: Used for hosting the backend API, providing a fully managed platform for building, deploying, and scaling web apps.
- **Azure PostgreSQL**: A cloud-based database service that ensures high availability and performance for data management.

#### Calendar Integration:
- **react-calendar**: A library used to implement the calendar view, allowing users to visualize their assignments and deadlines effectively.

### Architectural Decisions

- **Three-Tier Architecture**: The application follows a three-tier architecture consisting of:
  - **Presentation Layer (Frontend)**: Handles user interaction and presentation logic.
  - **Application Layer (Backend)**: Processes business logic and manages API endpoints.
  - **Data Layer (Database)**: Stores and manages application data.

- **RESTful API Design**: The backend is designed as a RESTful API, allowing for clear and standardized communication between the frontend and backend. This design facilitates easy integration and scalability.

- **Component-Based Frontend**: The frontend is organized into reusable components, promoting code reusability and maintainability. Each component encapsulates specific functionality, making it easier to manage and update.

### Key Features Implementation

#### Course Management:
- Implemented CRUD operations for courses using RESTful API endpoints. Users can add, edit, delete, and view courses through the Courses page.
- The course addition form validates input and formats URLs to ensure proper linking.

#### Assignment Tracking:
- Users can add assignments associated with specific courses. The assignment data is stored in the database and displayed in both the course view and the calendar.
- The completion status of assignments is tracked, allowing users to mark assignments as completed, which updates the visual indicators in the calendar.

#### Calendar View:
- The calendar displays all upcoming assignment deadlines with color-coded indicators for easy identification of pending and completed tasks.
- Real-time synchronization is implemented to ensure that any changes made in the Courses page are immediately reflected in the calendar view.

#### Minimization/Expand Courses:
- Added functionality to allow users to minimize and maximize course cards, improving the organization of the interface when managing multiple courses.
- This feature is implemented using local state management to track the minimized state of each course.

#### Testing:
- Unit tests are implemented for key components using React Testing Library, ensuring that individual parts of the application function correctly.
- End-to-end tests are conducted using Playwright to verify complete user workflows, ensuring that the application behaves as expected from a user's perspective.

#### Overall, the technical implementation of the Personal Learning Tracker application combines modern technologies and best practices to create a robust, user-friendly platform that effectively meets the needs of students managing their learning activities.
---

## 🚂 Development process

The development process for the **Personal Learning Tracker (PLT)** application was structured into several key phases, each building upon the previous one to create a comprehensive and functional tool for students. Below is a summary of the progress made from start to finish, highlighting key decisions and changes along the way.

### Phase 1: Definition and Planning
- **User Personas**: Identified target users, including exchange students, local university students, and part-time learners. This helped shape the application's features to meet their specific needs.
- **Use Cases**: Defined five core use cases that outlined the primary functionalities of the application, ensuring a clear understanding of user interactions.
- **Technical Architecture**: Established a three-tier architecture (frontend, backend, database) to ensure scalability and maintainability.

### Phase 2: Basic Structure and Main Functionalities
- **Frontend Development**: Started building the frontend using React. Implemented key components such as the Courses page and Calendar view, focusing on user-friendly interfaces.
- **Backend Development**: Developed the backend using Node.js and Express, creating RESTful API endpoints for managing courses and assignments. This included implementing CRUD operations.
- **Database Setup**: Initially set up a local PostgreSQL database for development and testing. This allowed for rapid iteration and debugging of features.
- **Integration**: Connected the frontend to the backend API, ensuring that data could be fetched and manipulated seamlessly.
- **Cloud Migration**: Migrated the database to Azure PostgreSQL for enhanced scalability and performance, allowing the application to handle multiple users effectively.
- **Deployment**: Finalized the deployment of the application on Azure, ensuring that both the frontend and backend were accessible and functional in a cloud environment.

### Phase 3: Extra Features and Improvements
- **Enhanced Calendar View**: Improved the calendar functionality to include visual indicators for assignment statuses and real-time synchronization with the Courses page. This was a significant enhancement aimed at improving user experience.
- **Minimization/Expand Feature**: Added the ability for users to minimize and maximize course cards, allowing for better organization when managing multiple courses. This decision was made based on user feedback regarding interface clutter.
- **Error Handling**: Implemented comprehensive error handling across both the frontend and backend to ensure a robust user experience. This included user-friendly error messages and appropriate HTTP status codes.

### Phase 4: Finalization and Presentation
- **Testing**: Conducted thorough testing, including unit tests for individual components and end-to-end tests to verify complete user workflows. This ensured that the application functioned correctly from a user's perspective.
- **Presentation**: Prepared a comprehensive presentation to showcase the application, highlighting its features, user interface, and the development process. The presentation included live demonstrations of key functionalities, allowing stakeholders to see the application in action and understand its value to users.

Overall,I nearly followed all the steps I planned in Phase 1, making only minor adjustments, such as adding the maximize/minimize feature to enhance the UI.

---

## ☀️ Reflection and Future Work

At first, creating the home, courses, calendar, and profile pages worked well and set a solid foundation for the application. However, I faced challenges with the database; while the structure I created can function, there are issues when attempting to retrieve the saved data. Additionally, migrating the database to Azure PostgreSQL presented challenges, particularly in optimizing the structure to better save and retrieve JSON data.

Currently, the application serves as my personal learning tracker. In the future, I plan to add registration and login functionality to allow other users to access the platform.

---

## 📊 Work Hours Log


| Date            | Time | Task                                           |
|-----------------|------|------------------------------------------------|
| 18.3.2025       | 3h   | Thinking about Phase 1                        |
| 20.3.2025       | 2h   | Planning Phase 1: Define Personas             |
| 21.3.2025       | 2h   | Planning Phase 1: Define Use Cases, Usage Scenarios, and UI Prototype |
| 21.3.2025       | 3h   | Planning Phase 1: Define Information Architecture and Technical Design |
| 22.3.2025       | 2h   | Planning Phase 1: Define Project Management and User Testing |
| 1.4.2025-12.4.2025 | 10h+ | Planning Phase 2: Frontend code               |
| 5.4.2025-13.4.2025 | 10h+ | Planning Phase 2: Backend code                |
| 5.4.2025-13.4.2025 | 5h   | Planning Phase 2: PostgreSQL database         |
| 1.4.2025-13.4.2025 | 5h   | Planning Phase 2: Testing and error handling  |
| 1.4.2025-13.4.2025 | 5h   | Planning Phase 2: UI/UX                       |
| 13.4.2025       | 2h   | Planning Phase 2: PostgreSQL Azure            |
| 13.4.2025       | 2h   | Planning Phase 2: Backend Azure               |
| 13.4.2025       | 4h   | Planning Phase 2: Frontend Azure              |
| 13.4.2025       | 4h   | Planning Phase 2: Phase 2 report              |
| 14.4.2025       | 4h   | Planning Phase 2: Fix minor issues            |
| 15.4.2025-27.4.2025 | 10h+ | Planning Phase 3: Make improvements and add features |
| 27.4.2025       | 3h   | Planning Phase 4: Presentation            |
| **Total**       | **76h+** |       

---

## 🪢 Presentation link

[_Add a link to state that it was presented live._](https://witty-water-006f88503.6.azurestaticapps.net)
