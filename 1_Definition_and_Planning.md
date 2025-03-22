# **Phase 1 - Definition and Planning**


## Table of Contents
[Project Overview](#project-overview)
1. [User Personas](#user-personas)
2. [Use Cases and Usage Scenarios](#use-cases-and-usage-scenarios)
3. [UI Prototypes](#ui-prototypes)
4. [Information Architecture and Technical Design](#information-architecture-and-technical-design)
5. [Project Management and User Testing](#project-management-and-user-testing)

## Project Overview
### **Project Name:** Personal Learning Tracker (PLT)

### **Objective:**
The Personal Learning Tracker (PLT) is a web-based application designed to help students manage and track courses, assignments, and class schedules from multiple universities and online platforms. In Finland, since students can enroll in courses from different universities and platforms like MOOC.FI, FITECH, EDX, and Coursera, it becomes difficult to track all course schedules and assignment deadlines in one place. PLT provides a centralized platform where students can input and view all course-related activities efficiently.

### **Key Features**
- **Course Management:** Add, edit, delete courses from different universities and platforms.
- **Assignment & Deadline Tracking:** Input assignments and deadlines.
- **Class Schedule Management:** Store and display class times.
- **Calendar View:** Display upcoming deadlines and class schedules in a weekly/monthly format.
- **Notifications:** Receive reminders for upcoming deadlines and classes.

---

## User Personas

### **Persona 1: Friend A, an Exchange Student**
- **Background:** An Erasmus exchange student in Finland.
- **Pain Points:** Needs to track courses from her home university and Finnish university.
- **Goals:** Wants a single calendar to manage all assignments and class schedules.

### **Persona 2: Friend B, a Local University Student**
- **Background:** A student enrolled in multiple Finnish universities through online courses.
- **Pain Points:** Struggles with keeping track of deadlines across different Moodle systems and online platforms. 
- **Goals:** Wants a tool to centralize all his coursework and deadlines.

### **Persona 3: Friend C, Studying Part-Time online**
- **Background:** A person who is working while taking online courses from different institutions.
- **Pain Points:** Finds it hard to balance work, study, and deadlines.
- **Goals:** Needs an efficient way to plan coursework around her job schedule.

---

## Use Cases and Usage Scenarios

### **Use Case 1: Adding a New Course**
**Actors:** Student  
**Scenario:** A student logs in and adds a new course by entering course details (name, university/platform, Moodle link, credits, etc.).

### **Use Case 2: Adding an Assignment Deadline**
**Actors:** Student  
**Scenario:** A student inputs an assignment deadline with a due date and course association. The deadline appears in the calendar.

### **Use Case 3: Viewing the Calendar**
**Actors:** Student  
**Scenario:** A student accesses the calendar to see upcoming class times and assignment deadlines.

### **Use Case 4: Editing Course Information**
**Actors:** Student  
**Scenario:** A student edits details of an existing course, such as changing the university name or updating the Moodle link.

### **Use Case 5: Receiving Notifications**
**Actors:** Student  
**Scenario:** A student receives a reminder notification for an upcoming assignment deadline or class.

---

## UI Prototypes
- **Dashboard:** Displays courses and upcoming deadlines.
  - Displays an overview of enrolled courses, upcoming deadlines, and scheduled classes.
  - Provides quick access to essential features such as adding a new course, viewing assignments, and managing notifications.
  - Includes a progress tracker to help students visualize their completed and pending coursework.
  - Allows users to customize their dashboard layout based on preferences (e.g., weekly view, priority tasks).

- **Course List Page:** Allows users to manage courses.
  - Displays a structured list of all courses added by the user, categorized by university or online platform.
  - Each course card contains essential details such as course name, university/platform, credits, and links to external resources (e.g., Moodle, MOOC.fi, Coursera).
  - Users can search, filter, and sort courses based on various attributes like institution, start date, or progress.
  - Provides options to add, edit, or delete course entries.

- **Calendar View:** Shows assignments and schedules.
  - A visual representation of assignment deadlines, class schedules, and important academic events.
  - Supports both weekly and monthly views to accommodate different planning preferences.
  - Integrates color-coded labels to differentiate between assignments, exams, and regular classes.
  - Allows users to set reminders and sync their schedules with external calendars like Google Calendar.
- **Add/Edit Page:** Input forms for courses and assignments.
  - Provides a simple and structured form for users to input new course details, assignment deadlines, and class schedules.
  - Features validation checks to prevent duplicate entries and incorrect date inputs.
  - Supports batch input for students adding multiple courses at the beginning of a semester.
  - Includes an auto-save function to prevent data loss during input.
- **Notifications & Reminders:** Customizaable notification setting.
  - Displays upcoming deadlines and sends reminder notifications based on user preferences.
  - Offers options for email, push notifications, or in-app alerts for critical deadlines.

*(Prototypes will be created using Figma.)*

---

## Information Architecture and Technical Design
### **Architecture Overview:**
- **Frontend:** Next.js (React) + TailwindCSS
- **Backend:** Firebase or Node.js (Express)
- **Database:** PostgreSQL or Firebase Firestore
- **Calendar Integration:** FullCalendar.js

### **Data Model:**
- **Courses:** id, name, university/platform, Moodle link, credits
- **Assignments:** id, title, due date, course_id
- **Schedule:** id, date, time, course_id

---

## Project Management and User Testing
- **Time Log:** Maintained in a separate GitHub page.
- **Development Phases:**
  - Phase 1: Definition and Planning
  - Phase 2: Basic structure and Main function
  - Phase 3: Advanced features and optimization
  - Phase 4: Presentation
- **User Testing Plan:**
  - Initial feedback from peers.
  - Usability testing with real users before release.
  - **Application Testing:**
    - **Unit Testing:** Individual components such as course addition and deadline input will be tested.
    - **End-to-End Testing:** Ensuring the complete workflow (adding courses, deadlines, and calendar view) functions correctly.
    - **Load Testing:** Evaluating performance with multiple concurrent users to check system stability.


