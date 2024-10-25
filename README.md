# Farm Help

## Overview

**Farm Help** is a full-stack application designed to assist farmers in making informed decisions regarding crop planting based on environmental data. This project integrates various technologies, including Node.js, Express, Mongoose, and React.js, alongside hardware components to provide real-time insights into flood and drought risks.

## Features

- **Data Collection**: 
  - Extracted flood data from NASA Worldview for each state over the past five years.
  - Analyzed drought trends using the U.S. Drought Monitor to identify at-risk months.
  - Researched crop data focusing on environmental conditions impacting agriculture.

- **Backend Server**:
  - Built with Node.js and Express, featuring endpoints for predicting floods and droughts based on date and state.
  - Developed APIs that recommend crops based on flood and drought risks, as well as soil conditions (temperature, humidity, soil moisture).

- **Real-time Data Integration**:
  - Set up a server to connect to an Arduino via a serial port using Socket.io.
  - Collected real-time environmental data (temperature, humidity, soil moisture) from a DHT22 sensor and other sensors.

- **Responsive Frontend**:
  - Developed a user-friendly interface using React.js that allows users to interact with the system, view predictions, and access recommendations.

## Technologies Used

- **Frontend**: React.js
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Real-time Communication**: Socket.io
- **Hardware**: Arduino, DHT22 sensor, soil moisture sensor

## Getting Started

### Prerequisites

- Node.js
- MongoDB
- Arduino IDE (for hardware setup)

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yara-e/farm-help.git
    cd farm-help
    ```

2. **Install backend dependencies**:
    ```bash
    cd server
    npm install
    ```

3. **Install frontend dependencies**:
    ```bash
    cd ../client
    npm install
    ```

4. **Set up MongoDB**:
   - Ensure MongoDB is running and configure the connection string in the server.

5. **Run the servers**:
   - Start the backend server:
     ```bash
     cd server
     npm start
     ```
   - Start the frontend server:
     ```bash
     cd client
     npm start
     ```

6. **Connect the Arduino**:
   - Upload the Arduino code to your device to start sending sensor data.

## Usage

- Navigate to the frontend application in your browser (`http://localhost:5173`).
- Use the interface to check flood and drought predictions.
- Get crop recommendations based on real-time data.

## Acknowledgments

- NASA Worldview
- U.S. Drought Monitor
- Arduino Community
