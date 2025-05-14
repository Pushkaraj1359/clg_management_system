# 🎓 College Management System

A full-stack web application built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js) to manage the operations of a college including **Students**, **Teachers**, **Classes**, **Subjects**, **Attendance**, and **Fee Management**. The system includes **role-based access control** for Admins, Teachers, and Students, ensuring a secure and efficient workflow.

---

## 🚀 Features

### 👩‍💼 Admin
- Add/update/delete students and teachers
- Create and manage classes and subjects
- Assign teachers to subjects
- Set class-wise fee structure
- View reports on attendance, fee payments, and exam results

### 👨‍🏫 Teacher
- View and manage assigned subjects
- Mark and view student attendance
- Enter and update student exam results

### 👨‍🎓 Student
- View personal academic details
- Track attendance and exam results
- Pay fees online (Razorpay integration)
- Download receipts and check due dates



## 🛠️ Tech Stack

| Tech         | Description                            |
|--------------|----------------------------------------|
| **Frontend** | React.js, Redux, Material-UI           |
| **Backend**  | Node.js, Express.js                    |
| **Database** | MongoDB (Mongoose ODM)                 |
| **Authentication** | JWT-based secure auth            |



## 🧑‍💻 Installation

### 1. Clone the Repository

```bash
git clone  https://github.com/KiranKPoojary/College-Management-System_MERN-Stack.git
cd college-management-system
```

### 2. Setup Backend

```bash
cd backend
npm install
npm start
```

- Create a \`.env\` file in the \`backend\` directory and add:

```bash
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

### 3. Setup Frontend

```bash
cd frontend
npm install
npm start
```

The client will start on \`http://localhost:3000\`

---

## 💳 Payment Integration

- Razorpay can be integrated for real-time fee payments.
- On successful payment, the student's \`fees.status\` will be updated to \`"Paid"\` in MongoDB, and a transaction ID is stored.

---

## 🔒 Role-Based Access Control

| Role    | Permissions                                       |
|---------|--------------------------------------------------|
| Admin   | Full control over all modules                    |
| Teacher | Manage subjects, attendance, and results         |
| Student | View data and pay fees                           |



## 🧪 Future Enhancements

Generate PDFs for fee receipts and academic results

Interactive admin dashboard featuring data visualizations

Automated email and SMS alerts for pending fees and attendance updates

Dedicated login portal for parents to monitor student information


