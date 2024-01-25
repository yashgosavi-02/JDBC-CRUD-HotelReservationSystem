# JDBC-CRUD-HotelReservationSystem

Welcome to the Hotel Reservation System, a simple Java application for managing hotel reservations.

## Overview

This system allows users to perform various actions related to hotel reservations, such as reserving a room, viewing reservations, getting room numbers, updating reservations, and deleting reservations. It utilizes a MySQL database for storing reservation data.

## Prerequisites

- Java Development Kit (JDK)
- MySQL Database
- MySQL Connector/J (JDBC Driver)

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/hotel-reservation-system.git

2. Set up your MySQL database and update the connection details in the Main.java file:
  ```bash
   private static final String url = "jdbc:mysql://localhost:3306/db_name";
   private static final String username = "username";
   private static final String password = "password";
  ```
3. Compile and run the application:
   ```bash
   javac Main.java
   java Main
   ```

## Usage
Choose an option from the main menu:

1: Reserve a room

<img width="408" alt="image" src="https://github.com/yashgosavi-02/JDBC-CRUD-HotelReservationSystem/assets/90139024/03fd1636-6567-4490-94e5-c55ccb00001a">

2: View Reservations

<img width="714" alt="image" src="https://github.com/yashgosavi-02/JDBC-CRUD-HotelReservationSystem/assets/90139024/12345542-8bff-450e-aa29-85552b180234">

3: Get Room Number

<img width="497" alt="image" src="https://github.com/yashgosavi-02/JDBC-CRUD-HotelReservationSystem/assets/90139024/5a631a43-e171-4491-97c3-83db1a05d669">

4: Update Reservations

<img width="512" alt="image" src="https://github.com/yashgosavi-02/JDBC-CRUD-HotelReservationSystem/assets/90139024/3e4520f2-8d8b-4f9e-98c8-d9059273b082">

5: Delete Reservations

<img width="514" alt="image" src="https://github.com/yashgosavi-02/JDBC-CRUD-HotelReservationSystem/assets/90139024/3e0a2222-1335-4fbd-8c45-332669a8de0e">

6: Exit

<img width="435" alt="image" src="https://github.com/yashgosavi-02/JDBC-CRUD-HotelReservationSystem/assets/90139024/3ff2670b-9ae4-4c12-b41b-7c36ee9fd68e">

Follow the prompts to perform the selected action

## Database Schema
The system uses a MySQL database with the following schema:
```bash
  CREATE TABLE reservation (
      reservation_id INT PRIMARY KEY AUTO_INCREMENT,
      guest_name VARCHAR(255) NOT NULL,
      room_no INT NOT NULL,
      contact_no VARCHAR(15) NOT NULL,
      reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
  );
```


