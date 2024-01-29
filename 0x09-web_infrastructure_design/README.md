0x09-web_infrastructure_design
# Simple Web Stack Project

This project involves designing a simple web infrastructure with a one-server setup. Follow the steps below to understand and implement the design.

## Task 0: Simple Web Stack

### Whiteboard Design:

![Web Stack Diagram](<https://imgur.com/UDP6gsQ>)

### Components:

- **Server (IP: 8.8.8.8):**
  - Represents the physical or virtual machine hosting the entire infrastructure.

- **Domain Name: foobar.com**
  - A human-readable alias for the server's IP address.

- **DNS Record: www (CNAME)**
  - Configured to point www.foobar.com to the server's IP (8.8.8.8).

- **Web Server (Nginx):**
  - Handles HTTP requests, serves static content.
  - Acts as a reverse proxy, forwarding requests to the application server.

- **Application Server:**
  - Executes dynamic code, processes requests, generates dynamic content.
  - Communicates with the web server.

- **Application Files (Code Base):**
  - Codebase of the website stored on the server, accessed by the application server.

- **Database (MySQL):**
  - Stores and manages website data.
  - Accessed by the application server for data retrieval and updates.

### Communication:

- User requests www.foobar.com.
- DNS resolves www.foobar.com to the server's IP (8.8.8.8).
- Server communicates with the user's computer over HTTP/HTTPS.
- Web server forwards requests to the application server for dynamic content.

### Explanation of Roles:

- **Server:** Hosts the entire infrastructure.
- **Domain Name:** Provides a human-readable alias for the server's IP.
- **DNS Record (www):** Points the domain www.foobar.com to the server's IP.
- **Web Server (Nginx):** Handles HTTP requests, serves static content, acts as a reverse proxy.
- **Application Server:** Executes dynamic code, processes requests, communicates with the database.
- **Database (MySQL):** Stores and manages website data.

### Issues with Infrastructure:

- **SPOF (Single Point of Failure):** Any component failure may result in website unavailability.
- **Downtime during Maintenance:** Restarting the web server for code deployment may cause temporary downtime.
- **Scalability Issues:** Difficult to handle a large amount of incoming traffic.

### Image Hosting:

- Take a screenshot of the whiteboard diagram.
- Upload the screenshot to an image hosting service (e.g., Imgur).
- Insert the link to the screenshot below:

![Whiteboard Screenshot](<https://imgur.com/UDP6gsQ>)

### GitHub Submission:

- Push the README.md file to your GitHub repository.
- Insert the GitHub repository link in the provided URL box.

