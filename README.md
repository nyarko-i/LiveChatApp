# Flask Chat Application

This repository contains a simple Flask-based chat application that allows users to create and join chat rooms to communicate in real-time using Socket.IO.

## Features

- **Room Creation and Joining**: Users can create new chat rooms or join existing ones by entering a room code.
- **Real-time Messaging**: Utilizes Socket.IO to enable real-time messaging between users within the same chat room.
- **Dynamic Room Codes**: Randomly generates unique room codes for newly created rooms.
- **User Interaction**: Tracks the number of members in each room and displays messages sent by users.
- **Disconnect Handling**: Manages user disconnections from the chat rooms gracefully.

## Implementation

### Technologies Used

- **Flask**: Python web framework used for routing and handling HTTP requests.
- **Flask-SocketIO**: Integration for WebSocket support in Flask for real-time communication.
- **Random and String Libraries**: Utilized for generating random room codes.

### Components

- **`app.py`**: Contains the main Flask application with routes and Socket.IO event handling.
- **`templates/`**: Folder containing HTML templates for different pages (home, room, chatroom).
- **`static/`**: Directory for storing static files like CSS or client-side JavaScript (not included in this code snippet).

### Application Flow

1. **Home Page**: Users are prompted to enter a name and either join an existing room by providing a code or create a new room.
2. **Room Page**: Upon successful entry into a room, users can see existing messages and send messages to the chat.
3. **Socket Events**: Events like message sending, connection, and disconnection are handled using Socket.IO for real-time updates.

### Running the Application

1. Clone this repository.
2. Install the required dependencies (`Flask`, `Flask-SocketIO`).
3. Run the `app.py` file.
4. Access the application via a web browser using the provided URL (by default, `http://localhost:5000`).

### Example Usage

1. Navigate to the home page.
2. Enter a name and create or join a room using the provided form.
3. Interact with other users in the same room by sending and receiving messages in real-time.
