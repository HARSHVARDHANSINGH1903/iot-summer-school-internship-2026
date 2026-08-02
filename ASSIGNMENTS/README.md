# 📚 Internship Assignments

Welcome to the **Assignments** directory of the IoT Summer School Internship 2026 repository. 

This folder contains the weekly practical assignments, laboratory exercises, and script configurations completed during the 42-day Summer Internship at **Techible under i3c, IIT Jammu**. These assignments serve as the building blocks for the final integrated IoT Web Dashboard project.

## 📂 Folder Structure & Contents

*(Files and source code for the following modules are uploaded within this directory)*

*   **Assignment 1: Environment & Hardware Setup**
    *   Familiarization with microcomputing hardware.
    *   Ubuntu OS configuration and GPIO pin mapping.
    *   Basic Git and GitHub repository initialization.
*   **Assignment 2: Embedded Communication & I2C Protocol**
    *   Interfacing physical sensors using the I2C bus.
    *   Python and Node.js scripts for raw data acquisition.
    *   Solving power grounding and signal integrity issues.
*   **Assignment 3: Backend API Development**
    *   Setting up a local Node.js server using Express.js.
    *   Routing hardware telemetry to `localhost:3000`.
    *   Creating RESTful API endpoints for JSON data streams.
*   **Assignment 4: Frontend Dashboard Integration**
    *   Developing the `index.html` user interface.
    *   Utilizing the Fetch API for asynchronous, real-time data rendering without page reloads.
*   **Assignment 5: Advanced Hardware Troubleshooting**
    *   Debugging video stream errors (e.g., Raspberry Pi Camera Module).
    *   Analyzing Ubuntu kernel logs and utilizing I2C detection tools.

## 🛠️ Technologies & Tools Used
*   **Hardware:** ESP32, Raspberry Pi, Custom PCB (EasyEDA Pro)
*   **Software/OS:** Ubuntu, Node.js, Express.js, Python, C++
*   **Protocols:** I2C, UART, HTTP, REST
*   **Frontend:** HTML5, CSS3, Vanilla JavaScript

## 🚀 How to Use
Navigate into any specific assignment file to view the source code. To run the backend scripts locally, ensure you have Node.js installed and execute the following from the root of the project:

```bash
npm install
node server.js
