# Spring Boot Web Application with DeepSeek AI & Ollama

## Overview
This web application is built using Spring Boot and integrates DeepSeek AI locally with the help of Ollama. The integration is facilitated through Spring AI, providing seamless communication between the application and the AI model.

## Features
- Local execution of DeepSeek AI
- Integration with Ollama for AI model management
- Spring AI support for enhanced interaction with the model
- RESTful API endpoints for AI-powered features
- Scalable and modular architecture

## Prerequisites
Ensure you have the following installed:
- Java 17 or later
- Spring Boot 3+
- Ollama installed and configured
- DeepSeek AI model set up locally

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Iamanajaz/deepseek_springboot
   cd deepseek_springboot
   ```

2. Build the application:
   ```sh
   ./mvnw clean package
   ```

3. Run the application:
   ```sh
   java -jar target/deepseek_springboot.jar
   ```

## Configuration
Modify the application properties to suit your setup:
```properties
spring.application.name=deepseek_springboot
spring.ai.ollama.chat.options.model=deepseek-r1:latest

management.endpoints.web.exposure.include=*
management.info.env.enabled=true

info.app.name=deepseek_springboot
info.app.description=DeepSeek AI chatbot project for Spring Boot
info.app.version=0.0.1-SNAPSHOT
```
Ensure Ollama is running and DeepSeek AI is loaded before starting the application.

## API Endpoints
| Method | Endpoint      | Description              |
|--------|-------------|--------------------------|
| POST   | /api/chat   | Send a message to AI     |
| GET    | /api/status | Check application status |

## Usage
- Start the Ollama service
- Ensure the DeepSeek AI model is running
- Run the Spring Boot application
- Use the API to interact with AI capabilities

## Contributing
Feel free to fork this repository, create a feature branch, and submit a pull request.

## License
This project is licensed under the MIT License.

## Contact
For issues and contributions, open an issue on GitHub or reach out via email at amanajaz990@gmail.com