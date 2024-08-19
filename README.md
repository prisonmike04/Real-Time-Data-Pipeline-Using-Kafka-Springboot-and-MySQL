# Real-Time Data Pipeline Using Kafka and MySQL

## Overview
This project tracks real-time changes on Wikimedia (the platform behind Wikipedia) and saves those changes in a MySQL database. It listens to Wikimedia's live feed—capturing edits, new pages, and updates—and records these events in a database.

## How It Works

### Real-Time Data Stream
- Wikimedia broadcasts every change happening on its platform in real-time through a public feed.
- Our system listens to this feed and captures these changes.

### Message Queue (Kafka)
- We use Apache Kafka as a message queue to handle the data stream efficiently.
- Kafka acts like a conveyor belt, ensuring that each change (message) is processed and stored correctly, even with high volumes of data.

### Storing Data
- Changes are captured from Kafka and saved into a MySQL database.
- MySQL organizes and stores the data for easy access and future analysis.

## Why Use This System?
- **Efficiency:** Kafka handles high volumes of changes without overwhelming the system.
- **Reliability:** The system continuously processes and records data without missing events.
- **Data Organization:** Stored data can be analyzed, used for reports, or built upon for further tools.

## Prerequisites
To run this system, you need:
- **Java:** The programming language used for development.
- **Kafka:** The message queue system managing real-time data.
- **MySQL:** The database used for storing changes.
- **Maven:** A build and management tool for the project.

