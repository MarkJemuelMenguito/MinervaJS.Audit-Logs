# MinervaJS.Audit-Logs 📜

![GitHub Release](https://img.shields.io/github/release/MarkJemuelMenguito/MinervaJS.Audit-Logs.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

Welcome to the MinervaJS.Audit-Logs repository! This module offers a simple and effective way to manage console messages for auditing, debugging, information, warnings, and errors. 

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Introduction

MinervaJS.Audit-Logs is designed for developers who need a reliable logging system. Whether you are tracking errors, debugging your application, or providing informational messages, this module helps you keep your logs organized and accessible. 

Logging is a crucial part of any application. It allows developers to monitor their applications and quickly identify issues. This module simplifies that process.

## Features

- **Audit Logs**: Keep track of all important events in your application.
- **Error Logging**: Capture and log errors for easier debugging.
- **Informational Messages**: Provide users with useful information during runtime.
- **Warnings**: Alert users about potential issues.
- **Easy Integration**: Simple to set up and use within any JavaScript project.

## Installation

To install MinervaJS.Audit-Logs, you can use npm. Run the following command in your terminal:

```bash
npm install minervajs-audit-logs
```

## Usage

After installing the module, you can easily import and use it in your JavaScript files. Here’s a basic example:

```javascript
const AuditLogs = require('minervajs-audit-logs');

// Initialize the logger
const logger = new AuditLogs();

// Log an informational message
logger.info('Application has started.');

// Log a warning
logger.warn('This is a warning message.');

// Log an error
logger.error('An error occurred while processing your request.');
```

You can customize the logger further to fit your needs. For detailed options and configurations, refer to the API Reference section below.

## API Reference

### Logger Methods

- **info(message)**: Logs an informational message.
- **warn(message)**: Logs a warning message.
- **error(message)**: Logs an error message.
- **audit(message)**: Logs an audit message for tracking purposes.

### Configuration Options

You can configure the logger with various options. Here’s an example:

```javascript
const logger = new AuditLogs({
    logLevel: 'info', // Set the log level (info, warn, error)
    logToFile: true,  // Enable logging to a file
    filePath: './logs/audit.log' // Specify the file path for logs
});
```

### Example

Here’s a complete example that shows how to use the logger:

```javascript
const AuditLogs = require('minervajs-audit-logs');

const logger = new AuditLogs({
    logLevel: 'info',
    logToFile: true,
    filePath: './logs/audit.log'
});

logger.info('Application started successfully.');
logger.warn('Low disk space warning.');
logger.error('Failed to connect to the database.');
logger.audit('User logged in.');
```

## Contributing

We welcome contributions to MinervaJS.Audit-Logs! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

Please ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Links

For the latest releases, visit the [Releases](https://github.com/MarkJemuelMenguito/MinervaJS.Audit-Logs/releases) section. Here you can download the latest version and view the changes made in each release.

You can also check the [Releases](https://github.com/MarkJemuelMenguito/MinervaJS.Audit-Logs/releases) section for updates and new features.

## Conclusion

MinervaJS.Audit-Logs provides a straightforward way to manage logs in your JavaScript applications. With its simple API and various logging methods, it can help you keep track of important events and errors in your application. 

Thank you for checking out MinervaJS.Audit-Logs! We hope you find it useful in your projects. If you have any questions or feedback, feel free to reach out.