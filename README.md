# Hotel Management System (SQL Project)

This mini-project is a basic hotel management system using SQL, designed to manage customers, rooms, and reservations. It includes SQL code for table creation, sample data insertion, and queries for common operations like viewing room availability, handling bookings, and updating reservation statuses.

## Project Structure

The project includes SQL commands for:
- Creating tables for `Customers`, `Rooms`, and `Reservations`
- Inserting sample data into these tables
- Executing queries to manage room availability, reservations, and customer information

## Database Design

### 1. `Customers` Table
Stores customer information.
- `customer_id`: Primary key, auto-incremented
- `first_name`, `last_name`: Customer's name
- `contact_number`: Optional contact number
- `email`: Unique email for customer identification

### 2. `Rooms` Table
Stores room details.
- `room_id`: Primary key, auto-incremented
- `room_number`: Unique room identifier
- `room_type`: Type of room, can be 'Single', 'Double', or 'Suite'
- `price`: Price per night for the room
- `status`: Room availability status (Available, Booked, Maintenance)

### 3. `Reservations` Table
Stores reservation details and links customers to rooms.
- `reservation_id`: Primary key, auto-incremented
- `customer_id`: References the `customer_id` from the `Customers` table
- `room_id`: References the `room_id` from the `Rooms` table
- `check_in`, `check_out`: Dates for reservation period
- `status`: Status of the reservation (Confirmed, Cancelled, Completed)

## Sample Data

The project includes initial sample data:
- Two customers in the `Customers` table
- Three rooms in the `Rooms` table
- Two reservations in the `Reservations` table, linking customers to rooms with booking dates

## SQL Queries

The following queries are included to demonstrate basic operations:
- **View Available Rooms**: List rooms currently available for booking
- **View All Reservations**: Display all reservations with customer and room details
- **Update Room Status After Booking**: Update a room's status to 'Booked' when reserved
- **Cancel a Reservation**: Update reservation status to 'Cancelled'
- **View All Customers, Rooms, and Reservations**: Display all entries in each table

## Usage

To use this project:
1. Set up an SQL database and run the table creation code.
2. Insert the sample data.
3. Use the provided queries to manage and view data as per the requirements.

## Future Improvements

Additional features can be implemented, such as:
- More advanced filtering for available rooms by date range
- Automatic updates of room status based on reservation status
- Detailed customer profiles with more fields

## License

This project is open-source and available for educational and non-commercial use.
