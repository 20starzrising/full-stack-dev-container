# SeniorGo: Full Stack Dev Container 

This repository contains a full-stack development environment using a Dev Container. It includes a frontend built with React, a backend using Node.js, and a DFINITY Internet Computer canister as the decentralized backend. The project also features real-time messaging, notifications, and various other functionalities.

## Features

- **React Frontend**: A modern frontend built with React.
- **Node.js Backend**: A robust backend using Node.js and Express.
- **DFINITY Canister**: A decentralized backend powered by DFINITY Internet Computer.
- **Real-Time Messaging**: WebSocket-based real-time chat functionality.
- **Notifications**: Notifications for new messages, connection requests, and updates.
- **Voice Assistant**: Voice command functionality for creating requests and other actions.
- **Social Feed**: A community social feed for sharing experiences.
- **Event Calendar**: A calendar for displaying community events.
- **Networking**: Features for adding, accepting, and managing friends or connections.
- **Emergency Button**: A quick access button for emergency alerts.

## Getting Started

### Prerequisites

- **Docker**: Ensure Docker is installed on your machine.
- **Node.js**: Ensure Node.js is installed on your machine.
- **Visual Studio Code**: Recommended for using Dev Containers.
- **DFX CLI**: Install the DFINITY SDK command-line tool.

### Setting Up the Dev Container

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Open in Visual Studio Code**:
   Open the repository in Visual Studio Code.

3. **Open the Dev Container**:
   - Press `F1` and select `Remote-Containers: Open Folder in Container...`.
   - Select the cloned repository folder.

4. **Install Dependencies**:
   Once inside the container, install the necessary dependencies:
   ```sh
   cd frontend && npm install
   cd ../backend && npm install
   npm install -g dfx-cli
   ```

5. **Start DFX**:
   Start the DFINITY canister:
   ```sh
   dfx start --background
   ```

6. **Deploy the Canister**:
   Deploy the canister:
   ```sh
   dfx deploy
   ```

7. **Start the Backend Server**:
   ```sh
   cd backend
   node index.js
   ```

8. **Start the WebSocket Chat Server**:
   ```sh
   node chat-server.js
   ```

9. **Start the React Frontend**:
   ```sh
   cd frontend
   npm start
   ```

## Project Structure

- **frontend/**: Contains the React frontend code.
- **backend/**: Contains the Node.js backend code.
- **.devcontainer/**: Configuration for the Dev Container.
- **src/**: Contains the DFINITY canister code.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.
