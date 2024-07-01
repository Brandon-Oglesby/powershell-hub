# PowerShell Hub

PowerShell Hub is a web-based front end for PowerShell Core, providing a real-time, interactive PowerShell terminal accessible via any web browser. This project leverages ASP.NET Core and SignalR to facilitate seamless communication between the web client and the PowerShell process running on the server. Designed to run in a Linux container, this solution brings the power and flexibility of PowerShell Core to a web interface, making it convenient to execute and manage PowerShell commands remotely.

### Features

- Web-Based Interface: Execute PowerShell commands directly from your web browser.
- Real-Time Communication: Instant feedback from the PowerShell process using SignalR.
- Cross-Platform: Utilizes PowerShell Core, ensuring compatibility across different operating systems.
- Containerized Deployment: Run the application in a Linux Docker container for easy deployment and scalability.
- Secure Execution: Commands are executed in a secure, isolated environment within the container.

### Technologies Used

- ASP.NET Core: Provides the web server and handles HTTP requests.
- SignalR: Facilitates real-time communication between the client and server.
- PowerShell Core: Executes commands and scripts on the server.
- Docker: Containerizes the application for consistent deployment across environments.

<br>

# Getting Started

### Prerequisites

- Docker installed on your machine.
- .NET Core SDK installed.

### Building the Docker Image

Clone the repository:

```sh

git clone https://github.com/BrandonOglesby/powershell-hub.git
cd powershell-hub
```

Build the Docker image:
```sh

docker build -t powershell-hub .
```

Run the Docker container:

```sh

docker run -d -p 8080:80 powershell-hub
```

### Accessing the UI

Open your web browser and navigate to http://localhost:8080 to start using the PowerShell Hub.
Usage

Enter a PowerShell command in the input box at the top of the page.
Click the "Execute" button to run the command.
View the output in real-time in the output section below the input box.

<br>

# Contributing

Contributions are welcome! Please fork the repository and submit pull requests for any features, bug fixes, or improvements.

<br>

# License
This project is licensed under the MIT License - see the LICENSE file for details.
