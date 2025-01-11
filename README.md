# Event Management System

This is a Python-based Event Management System that allows users to schedule and manage events across multiple halls. It uses the `pandas` library to store user data and provides functionalities for user login, event creation, and event display.

## Features

- User Sign Up and Login
- Event Creation with Prioritization
- Event Scheduling across Multiple Halls
- Event Display with Cancellation for Overdue Events

## Classes

### Event

Represents an event with the following attributes:
- `name`: Name of the event
- `priority`: Priority of the event (Lecture, Workshop, Club activity)
- `budget`: Budget for the event
- `deadline`: Deadline for the event completion
- `duration`: Duration of the event in days

### EventManager

Manages events across multiple halls:
- `num_halls`: Number of halls available for events
- `schedules`: List of schedules for each hall

#### Methods
- `add_event(event)`: Adds an event to the appropriate hall based on its schedule and priority.
- `display_events()`: Displays all events scheduled in each hall.

### User

Represents a user with the following attributes:
- `name`: Name of the user
- `event_manager`: An instance of EventManager to manage the user's events

## Usage

1. **Sign Up**: Create a new user account.
2. **Login**: Login with an existing user account.
3. **Add Event**: Create a new event with details such as name, priority, budget, deadline, and duration.
4. **Display Events**: View all scheduled events and any cancellations due to deadlines.
5. **Logout**: Logout from the current user account.


