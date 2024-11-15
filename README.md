# 📚 Library Management System  

## 📖 Description  
The **Library Management System** is a web-based application developed in PHP. It utilizes **Object-Oriented Software Engineering (OOSE)** principles to deliver a modular, reusable, and efficient system. This project automates library operations such as managing books, users, transactions, and sending due date notifications.  

---

## ✨ Features  
- 📚 **Book Management**  
  - Add, edit, delete, and view book records.  
  - Track book availability and issue status.  

- 👥 **User Management**  
  - Register and manage member details.  
  - Maintain user borrowing history.  

- 🔄 **Transaction Management**  
  - Issue and return books.  
  - Automate due date tracking and fine calculation.  

- 🔍 **Search Functionality**  
  - Search for books by title, author, or category.  

- 📊 **Reports**  
  - Generate reports on borrowed books, overdue returns, and user activity.  

- 🔔 **Send Notifications on Due Date** (New Feature)  
  - Notify users via email/SMS about approaching due dates for borrowed books.  
  - Helps reduce overdue returns and fines.  

---

## 🧩 Object-Oriented Concepts  

The system is designed using key **OOP principles**:  
- **Encapsulation**: Classes hide their data and expose only necessary methods for interaction.  
- **Inheritance**: Base classes (e.g., `Person`) are extended by specific classes (`Admin`, `Member`).  
- **Polymorphism**: Methods like `notifyUser()` behave differently for email or SMS notifications.  
- **Abstraction**: Core functionalities like book borrowing and notifications are abstracted into reusable classes.  

### Example Classes with Notification Feature  
- **`Notification`**: A base class for notification methods (e.g., email, SMS).  
- **`EmailNotification`**: Sends email notifications for due dates.  
- **`SMSNotification`**: Sends SMS reminders.  

---

## 🛠 UML Diagrams  

## 📦 Class Diagram

The class diagram represents key classes such as Book, User, Admin, and Transaction and their relationships.

## 🔄 Sequence Diagram

The sequence diagram shows the interaction between a user, system, and database during a book borrowing transaction.

## 🤝 Collaboration Diagram

This diagram illustrates how objects (like User and Book) collaborate to complete operations.

## 🏁 State Diagram

The state diagram highlights the lifecycle of a book, transitioning between available, issued, and returned states.

## 🔄 Data Flow Diagram (DFD)

The DFD outlines how data flows between the user, application, and database during key operations.

## 🔄 Activity Diagram

The activity diagram details the workflow for issuing a book, from login to confirmation.

---



## 🚀 Installation  

### Prerequisites  
- Local server: **XAMPP** or **WAMP**  
- PHP (>=7.4) and MySQL  
- Email/SMS setup:  
  - Email: Configure SMTP in `php.ini`.  
  - SMS: Integrate an SMS API (e.g., Twilio, Nexmo).  

### Steps  
1. **Clone the repository**:  
   ```bash  
   git clone https://github.com/Padmashiniramu/Library-management-system.git  
   cd Library-management-system  
   ```  

2. **Set up the database**:  
   - Open your MySQL database (e.g., phpMyAdmin).  
   - Create a new database (e.g., `library_db`).  
   - Import the `library_db.sql` file.  

3. **Configure the project**:  
   - Open the `config.php` file and update database and SMTP credentials:  
     ```php  
     define('DB_SERVER', 'localhost');  
     define('DB_USERNAME', 'root');  
     define('DB_PASSWORD', '');  
     define('DB_NAME', 'library_db');  
     define('SMTP_SERVER', 'smtp.gmail.com');  
     define('SMTP_PORT', 587);  
     define('SMTP_USER', 'your-email@example.com');  
     define('SMTP_PASSWORD', 'your-email-password');  
     ```  

4. **Run the application**:  
   - Place the project folder in your server's `htdocs` directory.  
   - Start the Apache and MySQL services.  
   - Access the application at:  
     ```  
     http://localhost/Library-management-system  
     ```  

---

## 🧪 Testing  

### Types of Testing  
The project includes the following types of testing to ensure its functionality, reliability, and usability:  

1. **Unit Testing**  
   - Verifies individual components or methods like adding a book, issuing a book, or calculating fines.  

2. **Integration Testing**  
   - Ensures smooth interaction between modules such as user registration, book management, and transactions.  

3. **Functional Testing**  
   - Checks the overall functionality, such as issuing books, returning books, and sending notifications.  

4. **Performance Testing**  
   - Measures system performance under load (e.g., multiple concurrent users performing transactions).  

5. **User Acceptance Testing (UAT)**  
   - Ensures the system meets user expectations and functional requirements.  

### Testing File  
The testing scenarios and results are documented in a dedicated **testing file** included in the repository:  

- File: `testing/LibraryManagementSystem_Testing_Documentation.pdf`  

---

## 🔮 Future Enhancements  
- Allow users to customize notification preferences (email/SMS).  
- Implement push notifications for mobile users.  
- Add a dashboard widget to display upcoming due dates.  

---
## "Happy Coding!"😊
