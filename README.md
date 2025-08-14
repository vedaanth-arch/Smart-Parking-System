# Smart Parking System

A command-line smart parking reservation system using SQLite and Python. Users can sign up, log in, reserve parking spots, visualize optimal paths, and receive notifications for reservation status.

## Features

- **User Authentication:** Sign up and log in with username and password.
- **Parking Reservation:** Reserve spots based on vehicle size and time.
- **Spot Availability:** System finds the nearest available spot.
- **Visualization:** Shows shortest path from entry to reserved spot using a graph.
- **Notifications:** Alerts for reservation start, cancellation (if not entered in time), and overstaying.
- **Reservation Management:** Cancel reservations, check your spot, mark entry/exit.
- **Multi-threaded Notifications:** Real-time reservation status updates.

## Requirements

- Python 3.x
- SQLite3
- matplotlib
- networkx

Install dependencies:
```sh
pip install matplotlib networkx
```

## Usage

1. Ensure `parking_system_new.db` is present and initialized with required tables.
2. Run the system:
   ```sh
   python parking_system.py
   ```
3. Follow the prompts to sign up, log in, and manage reservations.

## Main Menu Options

1. Create a Parking Reservation
2. Cancel a Reservation
3. Know Your Spot
4. Show Notifications
5. Enter Parking Lot
6. Exit Parking Lot
7. Exit Program

## Database Schema

- `users`: Stores user credentials.
- `vehicles`: Stores vehicle info.
- `parking_spots`: Stores spot info and coordinates.
- `reservations`: Stores reservation details and