# E-Learning Web

A PHP and MySQL learning management system developed as a final-year project, with a Bootstrap-based web interface for students and administrators.

## Features represented in the source

- Course browsing and course detail pages.
- Student registration, profiles, enrolled courses and lesson viewing.
- Administration pages for courses, lessons, students, feedback and sales reports.
- Legacy Paytm checkout integration, configured for the test environment.

These features are present in the recovered source. A full application runtime test has not yet been performed.

## Technology stack

| Layer | Technologies |
| --- | --- |
| Frontend | HTML, CSS, JavaScript, jQuery, Bootstrap |
| Backend | PHP with mysqli |
| Database | MySQL |

## Repository layout

```text
ELearning/             PHP application and frontend assets
ELearning/Admin/       Administration interface
ELearning/Student/     Student interface
ELearning/PaytmKit/    Legacy payment integration
SQL/lms_db.sql         Sanitized database schema, without user data
.env.example          Required environment variable names
E-Learning-Website.zip Original archive retained for history; do not use for setup
```

## Local development setup

1. Use a local PHP web server with the `mysqli` extension and a MySQL database. Exact supported versions require runtime verification.
2. Create an empty database named `lms_db` and import `SQL/lms_db.sql`.
3. Set `DB_HOST`, `DB_USER`, `DB_PASSWORD` and `DB_NAME` in the PHP server environment. `.env.example` documents the variable names; this application does not automatically load `.env` files.
4. Serve the `ELearning/` directory through your local PHP server and open `index.php`.
5. Register a new test student account. The sanitized schema contains no existing student or administrator login. Administrator provisioning must be reviewed locally; no default credentials are published.
6. Add your own test course images, student images and lesson media as needed. Paths used by the application include `image/stu/`, `lessonvid/` and `video/banvid.mp4`.

Payment configuration reads `PAYTM_MERCHANT_KEY`, `PAYTM_MERCHANT_MID` and `PAYTM_MERCHANT_WEBSITE` from the server environment. Keep test credentials private. Current compatibility of the legacy payment integration has not been verified.

## Source recovery and privacy

The browsable source was recovered from a readable local project copy. The older ZIP already in this repository failed an integrity check and is retained only as an original artifact.

The public recovery copy excludes database records, original merchant credentials, student images, screenshots containing account information, local editor configuration and bundled video files. The SQL file preserves the six-table schema and indexes without publishing accounts, passwords, transactions or feedback.

## Development status

This is a legacy educational portfolio project, not a production-ready service. Authentication, password handling, database queries, uploads and payments require a security review before deployment. No production deployment or passing runtime test is claimed.

## Planned enhancements

Multiple tutors, discussion forums, quizzes and live classes were listed as future enhancements in the original documentation.

## License and attribution

The repository includes an [MIT license](LICENSE). The recovered local README calls the application “iSchool”; that original application naming is retained in the source where present. Check third-party asset and payment library licenses separately.
