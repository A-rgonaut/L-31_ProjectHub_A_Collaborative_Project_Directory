# L-31 ProjectHub: A Collaborative Project Directory

![EJS](https://img.shields.io/badge/EJS-8C8C8C?style=for-the-badge&logo=ejs&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)

> Team implementation of a multi-user web application for online project management and sharing in the form of a directory.

## 📖 **Context**

This project was developed for the **Reti di Calcolatori** examination of Prof. **Biagio Lenzitti**, during the **2022/2023** Academic Year at the **Università degli Studi di Palermo**, **Computer Science (L-31, 2086)** course.

## 👥 **Authors**
_Andrea Spinelli - Marco Valenti - Raffaele Terracino_

## 🛠️ **Technologies Used**

*   **Languages:** EJS, PHP, JavaScript, HTML
*   **Frameworks/Libraries:** Bootstrap
*   **Databases:** MySQL

## 🚀 **Installation and Setup**

To run this project locally, you will need a web server environment with Apache, PHP, and a MySQL database. The easiest way to get this set up is by installing **XAMPP** or a similar software package.

### Prerequisites

*   [XAMPP](https://www.apachefriends.org/index.html) (or an alternative like WAMP, MAMP, LAMP)
*   A web browser (e.g., Chrome, Firefox)
*   Git (to clone the repository)

### Instructions

1.  **Clone the repository**
    ```bash
    git clone https://github.com/your-username/project-name.git
    cd project-name
    ```

2.  **Move the project to the web server's directory**
    Copy the entire project folder (`project-name`) into the `htdocs` directory of your XAMPP installation.
    *   On **Windows**: `C:\xampp\htdocs\`
    *   On **macOS**: `/Applications/XAMPP/htdocs/`
    *   On **Linux**: `/opt/lampp/htdocs/`

3.  **Set up the Database**
    *   Start the **Apache** and **MySQL** modules from the XAMPP control panel.
    *   Open your browser and navigate to `http://localhost/phpmyadmin`.
    *   Create a new database. For example, you can name it `project_manager_db`.
    *   Select the newly created database and go to the **Import** tab.
    *   Upload the `.sql` file located in the project's `db/` folder (e.g., `db/schema.sql` or `db/database.sql`). This will create the necessary tables.

4.  **Configure the Database Connection**
    The PHP code needs the credentials to connect to the database you just set up.
    *   Navigate to the `code/php/require/` folder.
    *   Find the database connection configuration file (it might be named `config.php`, `db_connect.php`, or similar).
    *   Open the file and update the credentials. For a standard XAMPP installation, they are typically:

    ```php
    // Example of what to look for and modify
    $servername = "localhost";
    $username = "root";
    $password = ""; // XAMPP's default password is an empty string
    $dbname = "project_manager_db"; // The name of the DB you created in step 3
    ```

5.  **Launch the application**
    You are all set! Open your browser and navigate to the URL corresponding to the project folder.
    
    `http://localhost/project-name/`

    The server should automatically load the `index.html` file, and the application will be up and running.
