This repository contains the backend code for an Online Food Order System, built using Spring Boot and Gradle. The system allows customers to browse restaurants, place orders, and make payments. It also provides administrative functionality for managing restaurant menus and orders.

Project Structure
The project is organized as follows:
src/main/java/: Contains the core Java source files, organized by packages (controllers, services, models, repositories).
src/main/resources/: Configuration files, including application.yml for environment setup and resource management.
build.gradle: The Gradle build file that manages project dependencies and tasks.
gradle/: Gradle wrapper files for build automation.

Features
User Registration and Authentication: Handles user signup, login, and session management.
Restaurant Management: Admins can create and manage restaurants and menus.
Order Management: Customers can place, modify, and track their orders.
Payment Integration: Secure payment processing using external payment services.
Order Notifications: Provides real-time order updates and history.

Local Development
Clone the repository:
git clone https://github.com/tcyanhao/socialaibackend.git

Set up the database:
Install and configure PostgreSQL or any other relational database.
