# File Management System — PHP & MySQL

**Information Management System Design Practice | Undergraduate Coursework**

This repository documents a web-based **File Management System** prepared for an undergraduate course at **Hubei University of Technology**. It brings together the PHP application files, a MySQL/MariaDB database export, and the academic project report.

The project explores how a database-backed web application can organize files and folders, support user accounts, and provide basic file-sharing workflows.

## Project Overview

The included source code provides interfaces and backend operations for:

- **User accounts:** Login and user administration, with administrator and regular-user roles.
- **Files:** Upload, list, rename, download, and delete files.
- **Folders:** Create, rename, and delete folders.
- **Organization:** Browse folders and search visible file and folder names.
- **Sharing:** Mark uploaded files as public for display in the shared-files view.
- **Dashboard:** Display basic counts of users and files.

These features are described from the repository's source code; they have **not been independently tested as a running deployment**.

## Technology Stack

| Area | Technologies |
| --- | --- |
| Backend | PHP, MySQLi |
| Database | MySQL / MariaDB |
| Frontend | HTML, CSS, JavaScript, jQuery |
| Interface components | Bootstrap, DataTables, Font Awesome |
| Local development environment | Apache and MySQL/MariaDB (for example, XAMPP or WAMP) |

## Repository Structure

```text
File-Management-System/
├── README.md
├── File Management System.pdf     # Academic project report
├── database/
│   └── fms_db.sql                 # Database schema and sample records
└── source code/
    ├── index.php                  # Main application entry
    ├── login.php                  # Login interface
    ├── admin_class.php            # Application actions
    ├── ajax.php                   # Action requests
    ├── db_connect.php             # Database connection
    ├── files.php                  # File and folder listing
    ├── download.php               # File download handler
    ├── users.php                  # User administration
    └── assets/                    # Styles, scripts, libraries, uploads
```

The `source code/` directory also contains additional PHP views and forms for managing files, folders, and users.

## Local Setup (Legacy Project)

1. Install a local PHP/Apache and MySQL/MariaDB environment, such as XAMPP or WAMP.
2. Place the **contents** of `source code/` in a web-accessible local folder, for example `htdocs/file-management-system/`.
3. Create a database named `fms_db` and import `database/fms_db.sql` through phpMyAdmin or a compatible SQL client.
4. Adjust the local database configuration in `db_connect.php` to match your environment.
5. Start Apache and the database server, then visit `http://localhost/file-management-system/login.php`.

**Compatibility note:** The repository preserves a legacy academic implementation. Some included frontend assets may need correction or replacement for a successful run in a modern development environment. The application has not been verified on current PHP versions.

**Security note:** The original implementation does not meet current security expectations for password storage, SQL query handling, or file-access authorization. Run it only in a controlled local environment for coursework or learning; do not expose it to the public internet without updating and reviewing those areas.

## Academic Documentation

- **Course:** Information Management System Design Practice
- **Institution:** Hubei University of Technology
- **Student:** Muntasir Md Fahim (王一然)
- **Report:** [File Management System — Academic Report](File%20Management%20System.pdf)

The report is retained alongside the source code as part of the coursework documentation.

## Acknowledgments and Use

This project was prepared in an academic learning environment, with support from classmates and educational resources. The repository also includes third-party interface libraries, which remain subject to their respective licenses and notices. Any additional identifiable source references can be included as they are confirmed.

This repository is shared for **coursework documentation and educational reference**. No new project-wide reuse license is granted here for material whose original permissions have not been established.
