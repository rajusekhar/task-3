# Task 3 – Enhanced Blog App with PHP & MySQL

This is the third task of my **Web Development Internship at ApexPlanet Software Pvt. Ltd.**  
The project extends the basic blog application from Task 2 with advanced features including **search**, **pagination**, **user-based post management**, and a clean modern UI.

---

## ✅ Features Added in Task 3.1

- 🔍 **Search Posts**: Search by title or content with highlighted results using `<mark>`
- 📄 **Pagination**: Only 5 posts displayed per page with page navigation
- 👤 **Post Author Display**: Each post shows the author's username
- 🔐 **Author-only Edit/Delete**: Only the user who created the post can modify it
- 🎨 **Enhanced UI**: Gradient background, card-style post layout, and responsive form design with custom CSS

---

## 📁 Project Structure

blog-app/
│
├── db.php # Database connection
├── index.php # Login & Registration form
├── login.php # Authenticate user
├── register.php # Register new users
├── logout.php # Logout user session
├── dashboard.php # Post dashboard with search + pagination
├── create.php # Add new post
├── edit.php # Edit a post
├── delete.php # Delete a post
├── style.css # Custom styling



## 💽 Database Setup

Run the following SQL in phpMyAdmin:

```sql
CREATE DATABASE blog;
USE blog;

CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(255) NOT NULL UNIQUE,
  password VARCHAR(255) NOT NULL
);

CREATE TABLE posts (
  id INT AUTO_INCREMENT PRIMARY KEY,
  title VARCHAR(255) NOT NULL,
  content TEXT NOT NULL,
  user_id INT,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
If you already had the posts table from Task 2, just run:

sql
Copy
Edit
ALTER TABLE posts ADD COLUMN user_id INT AFTER content;
🚀 How to Run
Download XAMPP

Start Apache & MySQL

Import the database as shown above

Place the project folder inside htdocs

Open http://localhost/YOUR_FOLDER_NAME/index.php in your browser

🔗 Submission Links
📂 GitHub Repository: [Your GitHub URL here]

🎥 LinkedIn Video: [Your LinkedIn post URL here]

🙏 Thanks to
ApexPlanet Software Pvt. Ltd.
for providing this hands-on PHP & MySQL internship opportunity.

📞 Contact: +91 9905879870
🌐 Website: https://www.apexplanet.in/internship/

👨‍💻 Developer Info
Name: rajasekhar

LinkedIn:www.linkedin.com/in/
raja-sekhar-510983363


Email:lalsarraju@gmail.com 
