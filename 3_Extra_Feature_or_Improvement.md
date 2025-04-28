# Phase 3 – Extra Feature or Improvements (Optional)

## 🎯 Chosen Use Case or Feature to Improve
I chose to improve Use Case 3: Viewing the Calendar. The original definition was minimal, stating only "A student accesses the calendar to see upcoming class times and assignment deadlines." I transformed this into an interactive, visually rich calendar with real-time synchronization, visual status indicators, and immediate feedback on assignment status.

I selected this feature because effective deadline management is critical for student success. The enhanced calendar provides students with a comprehensive visual overview of their workload distribution and completion status, helping them prioritize their work and manage their time more effectively.

I also added a new feature to the Courses page allowing course minimization for better organization.

---

## 🔍 Original Definition

[Original Use Cases](https://github.com/supaizjy0321/PersonalLearningTracker/blob/main/1_Definition_and_Planning.md#2-use-cases-and-usage-scenarios)


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
