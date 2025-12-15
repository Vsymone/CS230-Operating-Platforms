# CS230-Operating-Platforms
# Draw It or Lose It – CS 230 Software Design Project
## Project Overview
This repository contains the completed software design document for *Draw It or Lose It*, a multi-platform, web-based game developed for the client **The Gaming Room** as part of the CS 230 Operating Platforms course. The project focuses on adapting an existing Android-only game into a scalable, cloud-ready application that supports multiple teams and players across desktop and mobile platforms.

## Client
**The Gaming Room**  
The Gaming Room is a game development company seeking to expand their game, *Draw It or Lose It*, into a distributed, web-based environment. The goal was to support concurrent users, ensure data integrity, and allow future scalability.

## Project Requirements
- Support multiple games, teams, and players
- Ensure unique names for games and teams
- Allow only one instance of the GameService in memory (Singleton pattern)
- Safely iterate through collections of games, teams, and players (Iterator pattern)
- Web-based deployment with cross-platform compatibility
- Support for multiple concurrent users

## System Architecture
The application is designed using a client-server architecture:
- **Client Tier**: Web browsers on desktop and mobile devices
- **Application Tier**: Server-side Java application managing game logic
- **Data Tier**: Relational database storing games, teams, and players
- **Communication**: HTTP/HTTPS with optional WebSocket support for real-time updates

## Design Patterns and OOP Principles
- **Singleton Pattern**: Ensures only one GameService instance exists in memory
- **Iterator Pattern**: Safely manages collections and enforces uniqueness
- **Inheritance**: Shared attributes implemented through a base Entity class
- **Encapsulation**: Private attributes with controlled access
- **Polymorphism**: Overridden methods such as `toString()` for consistent output

## Operating Platform Recommendation
Linux is recommended as the server-side operating platform due to its stability, scalability, cost effectiveness, and strong support for Java-based web applications. Client systems—including Windows, macOS, Android, and iOS—access the application through standard web browsers.

## Technologies Used
- Java
- Java Virtual Machine (JVM)
- Linux (recommended server platform)
- Relational Database (PostgreSQL or MySQL)
- HTTP/HTTPS
- GitHub for version control

## Security Considerations
- Encrypted client-server communication using HTTPS/TLS
- Authentication with hashed credentials and token-based sessions
- Input validation to prevent SQL injection and cross-site scripting
- Regular updates to the operating system and application dependencies

## Reflection
This project demonstrates my ability to analyze software requirements, design scalable architectures, and apply object-oriented principles and design patterns. Creating the design document before implementation helped clarify system behavior, reduce risk, and ensure the solution met both technical and user requirements. This artifact represents my understanding of operating platforms and cloud-based software design.

## Course Information
**Course:** CS 230 – Operating Platforms  
**Project:** Draw It or Lose It Software Design Document
