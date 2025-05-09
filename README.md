![image](https://github.com/user-attachments/assets/7adf64ca-35ac-49d2-9fcf-3ebe121d3abc)# airbnb-clone-project
The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. 
It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security.

#Team Roles And Responsibilities.
Frontend Developer
Backend Developer
Database Administrator
Devops Engineer
UI/UX Designer
Project Manager
QA Tester
Security Engineer

# Technology Stack
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Javascript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![Boostrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![Python](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=green)
![GrapQL](https://img.shields.io/badge/GraphQl-E10098?style=for-the-badge&logo=graphql&logoColor=white)
![PostGreSql](https://img.shields.io/badge/PostgreSQL-green?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)

HTML: *markup language for structuring pages*

CSS3 : *Styling for layout and responsiveness*

JavaScript: *(Vanilla or with a framework like React.js) – For interactivity and dynamic components*

Bootstrap: *Optional frameworks for responsive design*

Python: *Core programming language*

Django: *a web framework for building RESTful APIs*

GraphQL: *a query language for APIs, allows developers to make requests to fetch data from multiple data sources with a single API call*

PostgreSQL: *communicates with the database servers using objects codes. It's an (ORDMBS)*

Docker: *Containerization for consistent development and deployment*

Github: *For version control and collaboration*


# Database Design Overview

USERS == *Represents the platform’s users (both guests and hosts)*

=> *id (Primary Key)*

=> *username*

=> *email*

=> *password (hashed)*

=> *is_host (Boolean to differentiate between guest and host)*

PROPERTIES == *Represents a listing added by a host.*

=> *id (Primary Key)*

=> *user_id (Foreign Key to User)*

=> *title*

=> *description*

=> *location*

=> *price_per_night*

BOOKINGS == *Represents a reservation made by a guest.*

=> *id (Primary Key)*

=> *user_id (Foreign Key to User – the guest)*

=> *property_id (Foreign Key to Property)*

=> *check_in_date*

=> *check_out_date*

=> *status (e.g., pending, confirmed, cancelled)*

REVIEWS == *Represents feedback left by a guest after a stay.*

=> *id (Primary Key)*

=> *user_id (Foreign Key to User)*

=> *property_id (Foreign Key to Property)*

=> *rating (e.g., 1–5 stars)*

=> *comments*

PAYMENTS == *Represents a transaction for a booking.*

=> *id (Primary Key)*

=> *booking_id (Foreign Key to Booking)*

=> *amount*

=> *payment_method*

=> *payment_status (e.g., completed, failed)*

🔁 Entity Relationships
A User can own multiple Properties (if they are a host).

A User can make multiple Bookings.

A Property can have multiple Bookings and Reviews.

A Booking belongs to one User (guest) and one Property.

A Payment is linked to one Booking.

A Review is linked to one User and one Property.

# ✨ Feature Breakdown

👤 USER MANAGEMENT == *Users can register, log in, and manage their profiles. Hosts and guests are differentiated by role, allowing for customized access and functionality depending on the user type.*

*Property Management*
*Booking System*

# API Security

# CI/CD Pipeline
