# Java Web Server Project

This repository contains a Java-based implementation of different types of web servers. The project is organized into three folders, each demonstrating a specific web server model. The performance of these web servers can be measured using [Apache JMeter](https://jmeter.apache.org/).

## Folder Structure

### 1. **Single-Threaded Web Server**
   - A basic implementation of a web server that handles one request at a time.
   - Suitable for understanding the fundamentals of web server operations.
   - **Use Case**: Ideal for learning purposes or scenarios with minimal concurrent requests.

### 2. **Multi-Threaded Web Server**
   - An advanced implementation where each request is handled in a separate thread.
   - Improves concurrency by enabling multiple client requests to be processed simultaneously.
   - **Use Case**: Suitable for moderate traffic scenarios.

### 3. **Thread Pool Web Server**
   - Implements a thread pool to manage a fixed number of threads.
   - Efficiently handles high traffic while maintaining control over resource usage.
   - **Use Case**: Suitable for high-concurrency environments where resource management is critical.

## Features

- **Core Concepts Covered:**
  - Networking with Java (using `Socket` and `ServerSocket`).
  - Multithreading.
  - Thread pool management.

- **Performance Testing:**
  - The web servers' performance can be measured using Apache JMeter.
  - Test scenarios can include:
    - Single-user request handling.
    - Simulating multiple concurrent users.
    - Stress testing under heavy load.

## How to Run the Servers and Clients

1. Clone this repository:
   ```bash
   git clone https://github.com/kajalchoudhary1003/MultiThreadedWebServer
   cd MultiThreadedWebServer
   ```

2. Navigate to the desired server folder (`SingleThreaded`, `MultiThreaded`, or `ThreadPool`).

3. Compile and run the server and client on different terminals:
   ```bash
   javac Server.java
   java Server

   javac Client.java
   java Client
   ```


## Performance Testing with JMeter

1. Install Apache JMeter: [Download Here](https://jmeter.apache.org/download_jmeter.cgi).

2. Create a test plan:
   - Add a thread group to simulate users.
   - Configure HTTP requests targeting your web server.

3. Analyze results:
   - Use JMeter's graphical tools to measure response times, throughput, and error rates.

4. Compare performance:
   - Test each web server implementation under similar load conditions.
   - Evaluate metrics such as latency, concurrency handling, and resource usage.


Happy coding! 🚀

