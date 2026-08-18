# SunDevilConnect — College Club & Event Management System

SunDevilConnect is a full-stack web application developed as an Arizona State
University CSE 460 class project.

The application was designed to help students discover and engage with campus
clubs and events while giving club officers and administrators role-specific
tools for managing organizations, events, memberships, notifications, and
requests.

I designed and developed the project end to end across the frontend, backend,
and database layers.

## Project Overview

The project covered the full software development lifecycle, beginning with
requirements analysis and system design and progressing through implementation,
integration, testing, and final presentation.

SunDevilConnect was built around three primary user roles:

- **Students** — browse clubs and events, register for events, request club
  membership, receive notifications, submit new-club requests, and flag content.
- **Club Officers** — manage club information, events, membership requests,
  officers, announcements, re-registration, and dissolution requests.
- **Administrators** — review club registration and dissolution requests,
  manage flagged content, oversee organizations, and send system-wide
  notifications.

The original project specification emphasized centralized event discovery,
club membership, role-based dashboards, event registration, and administrative
oversight.

## Technologies

### Frontend
- React
- JavaScript
- HTML
- CSS

### Backend
- Java
- Spring Boot
- REST APIs
- JDBC / JdbcTemplate

### Database
- MySQL
- SQL

### Development & Design
- Git / GitHub
- Eclipse
- Visual Studio Code
- Object-Oriented Design
- UML
- MVC
- Client-Server Architecture

## Architecture and Design

I selected a three-tier web architecture consisting of:

1. a React single-page frontend
2. a Java Spring Boot backend
3. a MySQL relational database

The frontend communicates with the backend through RESTful API calls, while the
backend separates request handling, business logic, and data-access concerns.

The project also applied object-oriented design principles and software design
patterns, including Factory, Observer, and Strategy.

## Key Features

### Student Experience

Students can:

- browse clubs and events
- register and unregister for events
- request club membership
- leave clubs
- receive notifications
- submit new club registration requests
- flag inappropriate content
- view personalized club and event information from a role-specific dashboard

### Officer Experience

Club officers can:

- create and manage events
- review membership requests
- manage club information and officers
- send club announcements
- submit club re-registration requests
- submit dissolution requests
- monitor relevant club activity

### Administrator Experience

Administrators can:

- approve or deny club registration and re-registration requests
- process dissolution requests
- review and manage flagged content
- oversee clubs and events
- send targeted or system-wide notifications

## Application Screenshots

### Login

Users authenticate through a common login page and are routed to the
appropriate dashboard based on their role.

![SunDevilConnect login](assets/screenshots/login.png)

### Student Dashboard

The student dashboard centralizes club memberships, event registrations,
notifications, club requests, and other student-specific activity.

![SunDevilConnect student dashboard](assets/screenshots/student-dashboard.png)

<!--
### Officer Dashboard

![SunDevilConnect officer dashboard](assets/screenshots/officer-dashboard.png)

### Administrator Dashboard

![SunDevilConnect administrator dashboard](assets/screenshots/admin-dashboard.png)

### Event Discovery

![SunDevilConnect event discovery](assets/screenshots/events.png)

### Club Discovery

![SunDevilConnect club discovery](assets/screenshots/clubs.png)
-->

## Software Design

The backend was organized into modular subsystems for areas such as users,
events, clubs, notifications, flagged content, and administrative requests.

The project used design patterns to keep those systems modular and extensible:

- **Factory Method** for creating role-specific user objects
- **Strategy Pattern** for interchangeable event sorting behavior
- **Observer Pattern** for notification-related updates

For example, event sorting was designed so that behaviors such as sorting by
category, date, location, paid/free status, or popularity could be changed
without embedding every variation directly into the UI or controller logic.

## Database Design

The MySQL database supported persistent storage for users, roles, clubs,
events, notifications, flagged content, registration requests, dissolution
requests, club memberships, event registrations, and notification recipients.

Relational tables and foreign-key relationships were used to connect users,
clubs, events, and role-specific data.

## Project Scope

The completed application included:

- a React single-page frontend
- a Spring Boot REST backend
- a MySQL relational database
- role-based dashboards
- club and event management
- event registration
- notifications
- administrative request workflows
- flagged-content management
- reusable object-oriented design patterns

The final implementation included seven controllers, eight backend subsystems,
and more than 70 backend classes.

## What I Learned

SunDevilConnect gave me experience taking a software system through the full
development lifecycle rather than focusing on only one layer of implementation.

I worked through requirements analysis, system modeling, architecture,
object-oriented design, frontend development, backend development, relational
database design, integration, and final presentation.

The project strengthened my understanding of how frontend, backend, and
database layers work together in a full-stack application and how design
decisions made early in development affect implementation and maintainability.

## Source Code

The original source code remains private because this project was completed as
university coursework.

This public repository is intended to document the project, its functionality,
and my experience designing and developing the application without publishing
the course solution.
