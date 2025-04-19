# ClientHub - CRM System in Java (Spring Boot)

**ClientHub** is a full-featured CRM (Customer Relationship Management) system written in Java using **Spring Boot**.  
It helps manage clients, meetings, documents, emails, tasks, and more in a professional, scalable, and extensible way.

---

## 🧩 Features (v1.0 MVP)

### 👥 Client Management
- **Add, Edit, Delete clients**: Full CRUD operations for managing clients.
- **View detailed client profile**: Including name, contact info (phone, email), description, and tags.
- **Tagging system**: E.g. "VIP", "Lead", "Prospect", "Partner", etc. for categorizing clients.
- **Search & Filtering**: Find clients by name, email, tags, etc.
- **Notes per client**: Store important notes or interactions for each client.

### 📁 File Upload (PDF, DOC, etc.)
- **Attach files to clients**: Upload files related to each client, such as contracts, invoices, etc.
- **Store files securely**: Files can be stored locally in the MVP, with an option for future cloud storage (e.g., Amazon S3).
- **List/download/delete uploaded documents**: Easy management of client documents.

### 📧 Email Integration (IMAP / POP3)
- **Connect to external inboxes**: Integrate with popular email providers like Gmail, Outlook.
- **Fetch emails related to specific clients**: Automatically or manually link incoming emails to the corresponding client.
- **Email Preview**: View sender, subject, and a preview of the email content.
- **Auto-link emails to client**: Automatically associate incoming emails based on the client’s email address.

### 📆 Calendar / Meetings
- **Schedule meetings**: Set up meetings with clients, including details like time, location, and agenda.
- **View calendar**: Daily, weekly, and monthly views of scheduled meetings and tasks.
- **Reminders/notifications**: (Future feature) Get reminders for upcoming meetings or tasks.
- **Sync with Google Calendar**: (Optional future feature) Allow synchronization of meetings with Google Calendar.

### ✅ To-Do List
- **Global and client-specific tasks**: Add tasks that are either global or tied to a specific client.
- **Task statuses**: Track progress with statuses like **Pending**, **In Progress**, **Completed**.
- **Due dates & reminders**: Set due dates for tasks and receive reminders.

### 🔐 Authentication & Roles
- **User registration and login**: Support for user authentication using **JWT** or **session-based** authentication.
- **Roles**: Define different user roles like **Admin**, **Sales**, and **Viewer** to control access to various parts of the CRM.
- **Access control**: Different permissions per module based on roles.

---

## 🛠️ Stack

- **Backend**: Java 17, Spring Boot 3, Spring Security, Spring Data JPA, Lombok
- **Database**: PostgreSQL (default) or MySQL (optional)
- **File Storage**: Local storage (for MVP), S3-compatible cloud storage (optional future feature)
- **Email Integration**: JavaMailSender (IMAP/POP3 for fetching emails)
- **API Style**: RESTful API (JSON)
- **Testing**: JUnit 5 + Mockito for unit and integration tests

---

## 🚀 Getting Started

### Prerequisites

- **JDK 17** (or later)
- **Maven** or **Gradle** for building the project
- **PostgreSQL** or **MySQL** database (configured via `application.properties`)
