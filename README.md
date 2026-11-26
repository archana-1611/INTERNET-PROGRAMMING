# EduPortal - Institutional E-Learning & Timed Online Quiz Portal

An institution-grade, responsive e-learning portal designed for faculty to publish course curriculum materials and conduct automatically evaluated timed online quizzes. Students can enrol in courses, access unit-wise PDF guides and video lectures, attempt timed assessments with a live JavaScript countdown timer and auto-submission upon expiration, view real-time score evaluations, and track their learning history.

## 🚀 Live Netlify Deployment

This project is configured for one-click deployment on [Netlify](https://www.netlify.com/).

### Deployment Settings:
- **Build Command**: *(None required - static site)*
- **Publish Directory**: `.` (or root directory)
- **SPA Redirects**: Handled automatically via `_redirects` and `netlify.toml`

---

## 🌟 Core Features

### 🏛️ Faculty Portal
- **Course Management (CRUD)**: Create, edit, and delete academic courses with codes, titles, descriptions, and category tags.
- **Unit-Wise Study Materials**:
  - Add curriculum units.
  - Upload study materials categorized as **PDF Documents** or **Video Lecture Streams**.
  - Built-in preview modals and download triggers.
- **Timed Online Quiz Builder**:
  - Configure title, time limit (in minutes), and passing score threshold (`%`).
  - Add multiple-choice questions with 4 options, radio-based correct answer key designation, and solution explanations.
- **Student Performance & Gradebook**:
  - Filter scores course-wise and quiz-wise.
  - Search by student name and email.
  - Distinguishes between **Manual Submissions** and **Timeout Auto-Submissions**.
  - **Export to CSV**: Download student grade sheets in Excel-compatible CSV format.

### 🎓 Student Portal
- **Course Catalog & Enrollment**: Browse available courses and enrol with a single click.
- **Study Materials Hub**: Access unit-wise PDF study guides and video lectures with an embedded reader and download options.
- **Timed Online Quiz Engine**:
  - **Live JavaScript Countdown Timer**: Dynamic `MM:SS` timer display with a visual progress bar.
  - **Pressure Warning**: Progress bar and timer shift from indigo to amber and then to pulsating crimson red under 15 seconds.
  - **Auto-Submit on Timeout**: When the countdown reaches `00:00`, inputs are immediately locked, all answered questions are evaluated, the submission is recorded, and the user is redirected to the results page.
  - **Question Palette**: Quick jump grid with real-time status indicators (Answered, Flagged, Unanswered, Current).
- **Instant Evaluation & Breakdown**:
  - Immediate score computation (Score, Percentage, Time Spent, and Pass/Fail status).
  - Celebratory confetti on passing score.
  - Detailed Question-by-Question breakdown comparing selected choice vs. correct answer with explanations.
- **My Progress**: Track enrolled courses, total quizzes taken, and average score percentage.
- **My Profile**: View and edit user details (Name, Email, Department, Student ID, Avatar, and Bio).

---

## 💻 Tech Stack
- **HTML5 & CSS3**
- **Tailwind CSS** (via CDN)
- **Vanilla JavaScript (ES6+)** with complete `localStorage` persistence
- **FontAwesome 6** icons
- **Canvas Confetti** for evaluation celebrations
