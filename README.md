# Rust Actix-Web Server with Rhai Scripting Integration 🚀

Welcome to the documentation for the Rust Actix-Web Server with Rhai Scripting Integration! This guide introduces you to a powerful Rust web server that integrates with the Rhai scripting language. Whether you're a developer or just curious, this project offers a unique approach to web development. Let's explore its features and capabilities! 🌐

## Table of Contents

- [Introduction](#introduction)
- [How it Works](#how-it-works)
- [Endpoints](#endpoints)
- [Rhai Integration](#rhai-integration)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project showcases a Rust web server built with Actix-Web, a popular Rust web framework. It offers two endpoints, `/multiply/{num1}/{num2}` and `/add/{num1}/{num2}`, where you can perform multiplication and addition operations by passing parameters in the URL.

## How it Works

The project operates as follows:

1. It defines two Actix-Web endpoints, `/multiply/{num1}/{num2}` and `/add/{num1}/{num2}`, which accept two numbers as URL parameters.
2. For each endpoint, it initializes a Rhai scripting engine.
3. The Rhai engine registers two functions, `num1` and `num2`, which return the numbers provided in the URL.
4. It loads and evaluates a Rhai script (`multiply.rhai` or `add.rhai`) that performs the desired operation.
5. The result is formatted and returned as a response.

## Endpoints

### Multiply Endpoint

- **URL**: `/multiply/{num1}/{num2}`
- **Description**: Multiplies two numbers provided in the URL.
- **Example**: `/multiply/5/3` returns `15`.

### Add Endpoint

- **URL**: `/add/{num1}/{num2}`
- **Description**: Adds two numbers provided in the URL.
- **Example**: `/add/5/3` returns `8`.

## Rhai Integration

This project showcases the integration of the Rhai scripting language into a Rust web server. Rhai allows you to write custom logic and calculations in scripting files (`multiply.rhai` and `add.rhai`) while still benefiting from the performance and safety of Rust.

## Usage

To use the Rust Actix-Web Server with Rhai Integration, follow these steps:

1. Ensure you have Rust and Cargo installed on your system.

2. Clone the repository and navigate to the project directory:

   ```bash
   git clone https://github.com/your-username/actix-web-rhai-server.git
   cd actix-web-rhai-server
   ```

3. Build and run the server:

   ```bash
   cargo run
   ```

   This will start the server at `http://127.0.0.1:8080`.

4. Use your favorite HTTP client or web browser to access the endpoints, e.g., `http://127.0.0.1:8080/multiply/5/3`.

5. Observe the results of multiplication and addition operations, computed dynamically through Rhai scripting.

## Contributing

Contributions are welcome! If you have ideas for improvements, additional features, or find any issues, please feel free to open a pull request. Let's collaborate to enhance this unique Rust web server.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the project according to the terms of the license.

---

Explore the Rust Actix-Web Server with Rhai Integration, combine the power of Rust with scripting, and build dynamic web applications with ease. Happy scripting and web development! 🚀🌐
