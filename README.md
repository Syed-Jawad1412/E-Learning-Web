# E-Learning Web

A PHP and MySQL e-learning web application created as a final-year project. The frontend uses HTML, CSS, JavaScript and Bootstrap for a web-based course learning experience.

## Project overview

The archived project lists course browsing, student profiles, lesson viewing and an administration area for managing course content and student records. These features are described by the existing documentation and archive index; they have not been verified by running the application.

## Technology stack

| Layer | Technologies |
| --- | --- |
| Frontend | HTML, CSS, JavaScript, Bootstrap |
| Backend | PHP |
| Database | MySQL |

## Repository status

The application was uploaded as `E-Learning-Website.zip` rather than browsable source files. An integrity check of the current archive failed with invalid ZIP file headers. Although its file index can be read, its application contents could not be reliably extracted.

The original archive has been retained unchanged. A fresh, valid copy of the source is required before the project can be restored, reviewed or run reliably.

## Expected source layout

The archive index indicates the following layout:

```text
ELearning/          PHP application, frontend assets and student pages
ELearning/Admin/    Administrative pages
ELearning/Student/  Student profile and lesson pages
SQL/lms_db.sql      Database export
website-images/    Project screenshots
```

These paths describe the archive contents; they are not currently available as extracted files in this repository.

## Local setup after source recovery

1. Restore a valid copy of the original application and SQL schema.
2. Review the SQL export for personal information and replace sample credentials before importing it into a local MySQL database.
3. Configure a local PHP web server with MySQL support.
4. Configure the database connection using local development credentials.
5. Review any payment integration configuration and use sandbox credentials only.
6. Open the application through the local web server and verify the student and administrator flows.

Exact PHP/MySQL version requirements and installation commands must be confirmed after source recovery. This README does not claim that the current archive is runnable.

## Planned enhancements

The original documentation identifies multiple tutors, student–tutor discussions, quizzes and live classes as future enhancements, rather than completed features.

## Screenshots

The previous README linked to screenshot files that are not committed as standalone repository assets. Add verified screenshots after the original source and images have been recovered.

## License

This repository includes an [MIT license](LICENSE). Review the licenses of bundled assets and third-party components separately.
