# 📋 Student Feedback & Evaluation System

A modern web application for collecting, managing, and analyzing student feedback on courses, instructors, and institutional services.

The system provides separate dashboards for students and administrators, allowing students to submit feedback and administrators to create forms, manage questions, and analyze responses through visual statistics.

---

## 🎯 Overview

The **Student Feedback & Evaluation System** is designed to improve communication between students and educational institutions.

Students can submit feedback about their learning experience, while administrators can create feedback forms, manage questions, and analyze responses to identify areas for improvement.

The application uses a modern React-based interface with role-based dashboards and browser-based data persistence.

### Key Benefits

| User | Benefits |
|------|----------|
| 👨‍🎓 Students | Submit feedback, view available forms, and access aggregated results |
| 👨‍💼 Administrators | Create forms, manage questions, and analyze student responses |
| 🏫 Institutions | Use feedback data to improve courses, teaching, and student satisfaction |

---

## ✨ Features

### 🔐 Authentication & Authorization

- Student and administrator registration
- Login with email and password
- Role-based access control
- Protected routes for authenticated users
- Password confirmation during registration
- Persistent login using browser storage
- Separate dashboards for students and administrators

### 👨‍🎓 Student Features

- View available feedback forms
- Open and complete feedback forms
- Answer rating-based questions
- Submit text-based feedback
- View aggregated feedback results
- View average ratings and response statistics
- Read recent comments
- Submit anonymous feedback

### 👨‍💼 Administrator Features

- Create custom feedback forms
- Add rating and text-based questions
- Mark questions as required or optional
- Remove questions from forms
- View all created feedback forms
- View response statistics
- Analyze average ratings using charts
- Read student comments
- Delete outdated or unused forms

### 📊 Analytics & Insights

- Average rating calculation
- Total response tracking
- Visual representation of ratings
- Bar charts using Chart.js
- Text response analysis
- Recent feedback display
- Instant updates after feedback submission

### 🎨 User Interface

- Modern gradient-based design
- Responsive layout
- Card-based dashboard interface
- Smooth animations and transitions
- Interactive buttons and form controls
- Clean navigation
- Mobile-friendly design

---

## 🛠️ Tech Stack

### Frontend

| Technology | Version | Purpose |
|------------|---------|---------|
| React | 18.2.0 | Building the user interface |
| React Router DOM | 6.20.0 | Routing and navigation |
| Chart.js | 4.4.0 | Data visualization |
| React-Chartjs-2 | 5.2.0 | React integration for Chart.js |
| React Icons | 4.12.0 | User interface icons |
| Axios | 1.6.2 | HTTP request handling |
| Vite | 5.0.8 | Development server and build tool |
| Tailwind CSS | 3.3.6 | Utility-first styling |

### Development Tools

| Tool | Purpose |
|------|---------|
| ESLint | Code quality and linting |
| PostCSS | CSS processing |
| Autoprefixer | CSS vendor prefixing |
| npm | Package management |

---

## 📁 Project Structure

```text
student-feedback-system/
│
├── public/
│   └── favicon.ico
│
├── src/
│   ├── assets/
│   │
│   ├── components/
│   │   ├── FeedbackForm.jsx
│   │   ├── FeedbackForm.css
│   │   ├── Navbar.jsx
│   │   ├── Navbar.css
│   │   └── ProtectedRoute.jsx
│   │
│   ├── context/
│   │   ├── AuthContext.jsx
│   │   └── FeedbackContext.jsx
│   │
│   ├── pages/
│   │   ├── AdminDashboard.jsx
│   │   ├── Auth.css
│   │   ├── Dashboard.css
│   │   ├── Home.jsx
│   │   ├── Home.css
│   │   ├── Login.jsx
│   │   ├── Register.jsx
│   │   └── StudentDashboard.jsx
│   │
│   ├── routes/
│   │   └── AppRoutes.jsx
│   │
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
│
├── .eslintrc.cjs
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

### 📂 Folder Responsibilities

| Folder / File | Description |
|---------------|-------------|
| `components/` | Reusable UI components |
| `context/` | Global authentication and feedback state |
| `pages/` | Main application pages |
| `routes/` | Application routing configuration |
| `assets/` | Images and other static assets |
| `App.jsx` | Main application component |
| `main.jsx` | Application entry point |
| `App.css` | Global application styles |
| `index.css` | Base styles and CSS variables |
| `package.json` | Project dependencies and scripts |

---

## 🚀 Installation

### Prerequisites

Make sure the following are installed on your system:

- **Node.js** v14.0.0 or later
- **npm** v6.0.0 or later
- A modern web browser such as Chrome, Firefox, Edge, or Safari

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/student-feedback-system.git
cd student-feedback-system
```

### Step 2: Install Dependencies

```bash
npm install
```

### Step 3: Start the Development Server

```bash
npm run dev
```

### Step 4: Open the Application

Open the URL shown in your terminal.

For a typical Vite project:

```text
http://localhost:5173
```

The application will automatically reload whenever you make changes to the source code.

### Build for Production

```bash
npm run build
```

### Preview the Production Build

```bash
npm run preview
```

---

## 💻 Usage

### 👨‍🎓 For Students

#### 1. Register an Account

- Open the application.
- Navigate to the **Register** page.
- Enter your name, email, student ID, and department.
- Select the **Student** role.
- Create your account.

#### 2. Login

- Enter your registered email and password.
- Access the Student Dashboard.

#### 3. Submit Feedback

- View the available feedback forms.
- Select a form.
- Answer the rating and text-based questions.
- Submit your feedback.

#### 4. View Results

- Open the results section.
- View average ratings and response statistics.
- Read recent comments when available.

---

### 👨‍💼 For Administrators

#### 1. Register as an Administrator

- Open the **Register** page.
- Enter your details.
- Select the **Admin** role.
- Create your account.

#### 2. Login

- Enter your administrator credentials.
- Access the Admin Dashboard.

#### 3. Create a Feedback Form

- Click **Create New Feedback Form**.
- Enter the form title and description.
- Add rating or text-based questions.
- Mark questions as required or optional.
- Save the form.

#### 4. Analyze Feedback

- Open a feedback form.
- View the number of responses.
- Analyze average ratings using charts.
- Read text-based responses and comments.

#### 5. Manage Forms

- Create new forms.
- Edit questions when supported.
- Delete outdated forms.
- Review feedback submitted by students.

---

## 👥 User Roles

### 👨‍🎓 Student

**Dashboard:** Student Dashboard

**Permissions:**
- View available feedback forms
- Submit feedback
- View aggregated results
- Read recent comments

### 👨‍💼 Administrator

**Dashboard:** Admin Dashboard

**Permissions:**
- Create feedback forms
- Add and remove questions
- Mark questions as required
- View statistics
- Analyze responses
- Delete feedback forms

---

## 🔑 Demo Credentials

For testing purposes, you can create accounts using the following credentials.

| Role | Email | Password |
|------|-------|----------|
| 👨‍💼 Admin | `admin@example.com` | `admin123` |
| 👨‍🎓 Student | `student@example.com` | `student123` |

> **Note:** These are example demo credentials. If the accounts do not already exist in your browser storage, register them first using the appropriate role.

### How to Create Demo Accounts

1. Open the application.
2. Navigate to the **Register** page.
3. Enter the demo email and password.
4. Select the appropriate role.
5. Submit the registration form.
6. Login using the created credentials.

---

## 📸 Screenshots

### 🔐 Login Page

The login page allows students and administrators to securely access their respective dashboards.

<!-- Add your login screenshot here -->

### 👨‍🎓 Student Dashboard

The Student Dashboard allows students to view available feedback forms and submit responses.

<!-- Add your student dashboard screenshot here -->

### 👨‍💼 Admin Dashboard

The Admin Dashboard allows administrators to create forms, manage questions, and analyze feedback.

<!-- Add your admin dashboard screenshot here -->

### 📝 Feedback Form

Students can answer rating-based and text-based questions through the feedback form.

<!-- Add your feedback form screenshot here -->

### 📊 Results & Analytics

The results section displays aggregated ratings and visual statistics.

<!-- Add your results screenshot here -->

---

## 🔄 How the System Works

The application follows a simple feedback collection and analysis workflow.

```text
┌──────────────────────┐
│   User Registration  │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   User Login         │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Role Verification  │
└──────────┬───────────┘
           │
      ┌────┴────┐
      ▼         ▼
┌──────────┐ ┌──────────┐
│ Student  │ │  Admin   │
│Dashboard │ │Dashboard │
└────┬─────┘ └────┬─────┘
     │             │
     ▼             ▼
┌──────────┐ ┌──────────────┐
│ Submit   │ │ Create Forms │
│Feedback  │ │ & Questions  │
└────┬─────┘ └──────┬───────┘
     │              │
     └──────┬───────┘
            ▼
┌──────────────────────┐
│   Data Stored in     │
│      localStorage    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Calculate Statistics│
│  & Display Results   │
└──────────────────────┘
```

### Application Flow

1. A user registers with a selected role.
2. The user logs in using their credentials.
3. The application verifies the user's role.
4. Students access the Student Dashboard.
5. Administrators access the Admin Dashboard.
6. Administrators create feedback forms.
7. Students submit responses.
8. Responses are stored in browser localStorage.
9. The application calculates statistics.
10. Results are displayed through charts and summaries.

---

## 💾 Data Storage

This project uses **localStorage** for data persistence.

### Why localStorage?

- No backend server is required.
- Data remains available after refreshing the browser.
- Suitable for demonstrations and prototypes.
- Easy to test locally.
- Simple data management for small-scale applications.

### Important Note

Since the application uses browser localStorage:

- Data is stored only in the current browser.
- Data is not automatically shared between different users or devices.
- Clearing browser storage removes the saved data.
- This implementation is suitable for learning, demonstrations, and prototypes.

---

## 🧩 Data Structure

The following examples show the type of data used by the application.

### 👤 User

```javascript
{
  id: "user_001",
  name: "Ananya Sharma",
  email: "student@example.com",
  password: "student123",
  role: "student",
  studentId: "STU2026001",
  department: "Computer Science",
  createdAt: "2026-09-01T10:30:00.000Z"
}
```

### 📝 Feedback Form

```javascript
{
  id: "form_001",
  title: "Course Evaluation Form",
  description: "Evaluate the teaching and learning experience.",
  questions: [
    {
      id: "q_001",
      text: "How would you rate the course content?",
      type: "rating",
      required: true
    },
    {
      id: "q_002",
      text: "What improvements would you suggest?",
      type: "text",
      required: false
    }
  ],
  createdAt: "2026-09-01T11:00:00.000Z",
  createdBy: "user_002"
}
```

### 📊 Feedback Submission

```javascript
{
  id: "submission_001",
  formId: "form_001",
  userId: "user_001",
  userName: "Ananya Sharma",
  userRole: "student",
  responses: {
    q_001: 5,
    q_002: "The course content was clear and well organized."
  },
  submittedAt: "2026-09-02T09:15:00.000Z"
}
```

### ⭐ Rating Example

```javascript
{
  question: "How would you rate the course content?",
  rating: 5,
  maximumRating: 5
}
```

### 📈 Example Statistics

```javascript
{
  formId: "form_001",
  totalResponses: 25,
  averageRating: 4.32,
  ratingDistribution: {
    1: 1,
    2: 2,
    3: 4,
    4: 8,
    5: 10
  }
}
```

---

## 🎨 Customization

### Changing Colors

Update the gradient colors in the CSS files.

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Adding New Question Types

Extend the `FeedbackForm` component to support additional question types.

```jsx
{question.type === 'rating' && (
  // Rating input
)}

{question.type === 'text' && (
  // Text input
)}

{question.type === 'multiple-choice' && (
  // Multiple-choice input
)}
```

### Modifying Default Forms

Edit the default forms in `FeedbackContext.jsx`.

```javascript
const defaultForms = [
  {
    id: "form_001",
    title: "Course Evaluation Form",
    description: "Evaluate the course.",
    questions: [
      {
        id: "q_001",
        text: "Rate the course content.",
        type: "rating",
        required: true
      }
    ]
  }
];
```

### Styling Customization

- Update global styles in `App.css`.
- Modify CSS variables in `index.css`.
- Update component-specific CSS files.
- Customize Tailwind CSS configuration if used.

---

## 🌐 Deployment

### Deploy to Vercel

```bash
npm install -g vercel
vercel
```

### Deploy to Netlify

```bash
npm run build
```

Upload the generated `dist` folder to Netlify.

### Deploy to GitHub Pages

```bash
npm install --save-dev gh-pages
```

Configure the deployment settings in `package.json`, then run the deployment script.

> **Note:** For a production application, a backend database and secure authentication system should be used instead of browser localStorage.

---

## 🤝 Contributing

Contributions are welcome!

### How to Contribute

1. Fork the repository.
2. Clone your fork.
3. Create a new branch.
4. Make your changes.
5. Test the application.
6. Commit your changes.
7. Push the branch.
8. Create a Pull Request.

### Example Commands

```bash
git clone https://github.com/your-username/student-feedback-system.git

cd student-feedback-system

git checkout -b feature/your-feature-name

git add .

git commit -m "Add new feature"

git push origin feature/your-feature-name
```

### Development Guidelines

- Use functional React components.
- Follow consistent naming conventions.
- Write clean and readable code.
- Reuse components where possible.
- Add appropriate error handling.
- Test features before submitting changes.
- Update documentation when necessary.

---

## 📄 License

This project is developed for educational and demonstration purposes.

You may modify and extend the project according to your requirements.

---

## 👩‍💻 Author

**Student Feedback & Evaluation System**

Built using **React, Vite, Chart.js, and localStorage**.

---

⭐ If you found this project useful, consider giving it a star!
