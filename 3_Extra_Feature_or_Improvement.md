# Phase 3 – Extra Feature or Improvements (Optional)

## 🎯 Chosen Use Case or Feature to Improve
I chose to improve Use Case 3: Viewing the Calendar. The original definition was minimal, stating only "A student accesses the calendar to see upcoming class times and assignment deadlines." I transformed this into an interactive, visually rich calendar with real-time synchronization, visual status indicators, and immediate feedback on assignment status.

I selected this feature because effective deadline management is critical for student success. The enhanced calendar provides students with a comprehensive visual overview of their workload distribution and completion status, helping them prioritize their work and manage their time more effectively.

I also added a new feature to the Courses page allowing course minimization for better organization.

---

## 🔍 Original Definition

[Original Use Cases](https://github.com/supaizjy0321/PersonalLearningTracker/blob/main/1_Definition_and_Planning.md#2-use-cases-and-usage-scenarios)

### All Use Cases Now:
Use Case 1: Adding a New Course
Actors: Student
Scenario: Student enters course name and course link, clicks "Add Course" button, and the new course appears in the list with 0 study hours and no assignments.
Use Case 2: Adding an Assignment Deadline
Actors: Student
Scenario: Student selects a course, enters assignment name and due date, clicks "Add Assignment" button, and the new assignment appears in the course's assignment list and calendar.
Use Case 3: Viewing the Calendar
Actors: Student
Scenario: Student views the calendar displaying all assignments with color-coded indicators (green for pending, pink for completed assignments), selects dates to see detailed assignment information, and uses visual icons (sun for today, rainbow for completed days).
Use Case 4: Tracking Assignment Completion
Actors: Student
Scenario: Student clicks the checkbox next to an assignment to mark it as completed, triggering visual changes (strikethrough, background color) and updating the calendar display.
Use Case 5: Editing Course Information
Actors: Student
Scenario: Student clicks "Edit" on a course, modifies the name and/or link in the form fields at the top, and clicks "Update Course" to save changes.
Use Case 6: Tracking Study Hours
Actors: Student
Scenario: Student increments or decrements study hours for a course in 0.5-hour intervals using the "+" and "-" buttons, with changes immediately reflected in the display.
Use Case 7: Deleting an Assignment
Actors: Student
Scenario: Student clicks the "Delete" button on an assignment, removing it from both the course view and the calendar.
Use Case 8: Deleting a Course
Actors: Student
Scenario: Student clicks the "Delete" button on a course, removing the course and all its assignments from the system.
Use Case 9: Accessing Course Materials
Actors: Student
Scenario: Student clicks on a course link, which opens the associated website in a new browser tab for easy access to course content.
Use Case 10: Minimizing/Maximizing Courses
Actors: Student
Scenario: Student clicks "Minimize" on a course card to collapse its details (showing only the course name), or "Expand" to view all information, assignments, and controls for that course.

---

## 🔄 Implementation

1. React Calendar integration with custom styling: I implemented the react-calendar library with extensive customization through CSS to create a visually distinctive and informative calendar.
2. Visual assignment indicators: I created a system of visual cues to represent assignment status:
Green background with dashed borders for days with pending assignments
Pink background for days with completed assignments
A sun icon to highlight the current day
Rainbow icons to indicate completed assignments
3. Real-time data synchronization: I implemented:
A polling mechanism that checks for updates every 2 seconds
A localStorage-based event system to detect changes from other components
A manual refresh button for immediate data retrieval
4. Database restructuring: When encountering issues with the original PostgreSQL setup, I had to carefully redesign the table structure while ensuring backward compatibility. I created a new study_sessions table with foreign key relationships to courses, preserving data integrity while expanding functionality.
5. Course minimization/maximization: Added the ability to collapse and expand individual course cards, significantly improving the interface when managing multiple courses.
