# Movie Ticket Management System (SRS + UML/DFD/ER Design)

## Overview
This project documents the end-to-end design of a web-based Movie Ticket Management (“Movie World”) system that enables users to book movie tickets online and supports administrators in managing movies, theatres, and show assignments. The work is documentation-focused and includes SRS, DFDs, ER modeling, UML diagrams, and screen/page specifications.

## Problem Statement
Manual ticket booking is time-consuming and inconvenient. The goal is to provide an online solution where users can view available movies and show timings, select seats, complete payment, and receive tickets—while administrators maintain theatres, movies, and schedules.

## Users and Modules
### 1) User Module
- User registration and login
- View now-playing/upcoming movies and theatre details
- Select movie → select timing/show → choose seats
- Price calculation (includes tax rules)
- Payment workflow
- Ticket generation and delivery (email)

### 2) Admin Module
- Admin login and privileged access
- Register/manage theatres
- Add/manage movies
- Assign movies/shows to theatres
- View assignments and booking information

### 3) Ticket Booking Module
- Seat availability display and reservation for a selected show
- Booking confirmation and ticket issuance
- Ticket cancellation support

## Core Functional Requirements
- Authentication (username/password)
- Movie selection
- Show timing selection
- Seat class and seat-number selection (only unreserved seats)
- Automated price calculation (class + quantity + tax)
- Payment handling (including OTP in the documented flow)
- Ticket generation and email delivery

## Non-Functional Requirements
- Performance depends on internet connectivity and device/browser capability
- Safety and security expectations:
  - users should not share credentials
  - OTP/card details must be handled carefully during payment
  - rules to prevent illegal ticket duplication

## Technology Notes (as documented)
- Frontend: HTML and JavaScript
- Web layer: ASP.NET (code-behind approach and server controls)
- Database: SQL Server
- Data connectivity: ADO.NET concepts (Connection, Command, DataReader, DataAdapter, Dataset)

## Design Deliverables Included
- Software Requirements Specification (SRS)
- Data Flow Diagrams (context + multi-level flows for admin, user, booking)
- Entity-Relationship (ER) diagrams for database modeling
- UML diagrams:
  - Use case diagrams
  - Sequence diagrams
  - Class diagrams
  - Activity diagrams
  - Collaboration diagrams
- Screen and page documentation linking UI pages to database operations
