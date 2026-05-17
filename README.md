# IRCTC Console Ticket Booking System

A command-line Java application that simulates a railway ticket booking system. This project demonstrates core Object-Oriented Programming (OOP) concepts, collection frameworks, and console-based user interaction using in-memory data structures.

## Features

* **User Authentication:**
  * Register new users with a username, password, full name, and contact details.
  * Secure login and logout functionality using in-memory session management.
* **Train Management:**
  * View a pre-populated list of available trains, including routes and total seat capacity.
  * Search for specific trains based on source and destination stations.
* **Ticket Booking Engine:**
  * Book tickets by selecting a Train ID and specifying the number of seats.
  * Automatic validation to ensure requested seats do not exceed available capacity.
  * Real-time deduction of available seats upon successful booking.
* **Ticket Management:**
  * View a personalized history of all booked tickets for the logged-in user.
  * Cancel tickets by Ticket ID, which automatically refunds the seat count back to the train's available capacity.

## Tech Stack

* **Language:** Java (Core Java / Java SE)
* **Architecture:** MVC-inspired layered architecture (Models, Services, Controller)
* **Data Storage:** In-memory Collections (`ArrayList`, `HashMap`)
* **Input/Output:** Standard `Scanner` class for CLI interactions

## Project Structure

The codebase is modular and organized into distinct packages:


src/

├── controller.main/

│   └── IRCTCAPP.java         # Main entry point and interactive console menu

├── Services/

│   ├── BookingService.java   # Core logic for searching, booking, and cancelling

│   └── UserService.java      # Logic for registration and session management

├── train/

│   └── Train.java            # Train entity model with seat tracking logic

├── ticket/

│   └── Ticket.java           # Ticket entity model with auto-incrementing IDs

└── user/
    └── User.java             # User entity model

* **How to Run**
  * Ensure you have the Java Development Kit (JDK) installed on your machine.

  * Clone or download the repository to your local machine.

  * Open a terminal or command prompt and navigate to the root directory of the project.

* **Compile the Java files:**

  *javac controller/main/IRCTCAPP.java Services/*.java train/*.java ticket/*.java user/*.java

* **Run the application:**
  *java controller.main.IRCTCAPP
  *Follow the on-screen prompts to register a user, log in, and start booking tickets.
