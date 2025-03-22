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
- **Course List Page:** Allows users to manage courses.
- **Calendar View:** Shows assignments and schedules.
- **Add/Edit Page:** Input forms for courses and assignments.

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


