# Communication Tracker Calendar Application

## Objective
To maintain strong professional relationships by keeping accurate records of interactions with other organizations. This React-based Calendar Application enables efficient tracking of communication with companies, ensuring timely and consistent follow-ups. The application provides a centralized platform to log past interactions, plan future communications, and manage engagement frequency based on predefined schedules.

---

## Features

### Admin Module
- **Company Management**
  - Add, edit, and delete companies.
  - Fields: Name, Location, LinkedIn Profile, Emails, Phone Numbers, Comments, Communication Periodicity.
- **Communication Method Management**
  - Define communication methods with attributes: Name, Description, Sequence, Mandatory Flag.
  - Default methods:
    1. LinkedIn Post
    2. LinkedIn Message
    3. Email
    4. Phone Call
    5. Other

### User Module
- **Dashboard**
  - Grid-like view of companies with columns:
    - Company Name
    - Last Five Communications
    - Next Scheduled Communication
  - Color-coded highlights:
    - Red: Overdue communication
    - Yellow: Communication due today
- **Interactive Features**
  - Tooltip displays notes/comments on hover over completed communications.
- **Communication Actions**
  - Log new communications with fields: Type, Date, Notes.
- **Notifications**
  - Displays overdue and due communications in grids.
  - Notification icon shows badge count for overdue/due communications.
- **Calendar View**
  - Visualize past communications and manage future communications with a calendar interface.

---

## Project Structure

### File Organization
```
root/
|-- public/
|-- src/
    |-- components/
        |-- notification.js
        |-- notificationCalendar.js
    |-- context/
        |-- data.js
    |-- routes/
        |-- adminModule.js
        |-- companies.js
        |-- userDashboard.js
    |-- css/
        |-- App.css
        |-- components/
            |-- notification.css
            |-- notificationCalendar.css
        |-- routes/
            |-- adminModule.css
            |-- userModule.css
            |-- dashboard.css
    |-- App.js
    |-- index.js
```

### Key Components
- **NotificationsPage**: Displays overdue and today’s communications.
- **CalendarView**: Provides a calendar interface for past and upcoming communications.
- **AdminModule**: Handles company and communication method management.
- **UserDashboard**: Displays the dashboard for communication tracking.

### Context API
- Centralized state management using `CommunicationContext`.
- State includes companies, communication methods, and communications.
- Actions: Add, update, delete companies; Add communications; Manage communication methods.

---

## Technologies Used
- **Frontend**: React.js, React Router, React-Big-Calendar
- **Styling**: CSS
- **State Management**: Context API, Reducer Pattern
- **Backend**: Java Spring Boot
- **Database**: MySQL

---

## Installation Steps

1. Install required packages:
   ```bash
   npm install react react-dom react-router-dom react-big-calendar moment moment-localizer lucide-react uuid
   ```
2. Start the development server:
   ```bash
   npm start
   ```

---

## Future Enhancements
- Add a Reporting and Analytics Module for actionable insights.
- Implement advanced authentication and authorization.

---

