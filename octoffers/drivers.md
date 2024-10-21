---
title: "Drivers"
weight: 1
---

### Overview

Selenium's drivers allows browser automation by acting as a bridge between programming languages and web browsers. These drivers execute automated tasks on various web platforms. Octoffers uses both Open Source and Private drivers.

### Supported Platforms

| Platform | Type    | Status            |
|----------|---------|-------------------|
| Djinni   | Public  | Complete          |
| Indeed   | Private | Beta              |
| WorkBC   | Public  | Under Development |
| Monster  | Public  | Under Development |


### Open Source Drivers

Open Source Drivers support popular browsers like Chrome and Firefox. They are maintained by a community and foster experimentation and innovation without licensing constraints.

### Private Drivers

Private Drivers are customized for specific needs, exclusive to Octoffers team members and subscribers. They offer advanced features and exclusive support, making them ideal for unique automation tasks.

### Reusable Modules in Octoffers

1. Modular Design: Functionality is summed up in reusable modules, such as the Driver class, which handles Web Driver management.

2. Profile Management: The Profile class allows users to manage multiple profiles efficiently.

3. Session Management: A centralized session module manages cookies and authentication across tasks, reducing repeated logins.

4. Error Handling & Logging: Standardized error handling and logging mechanisms improve troubleshooting and maintenance.

5. Scalability: New platforms can be integrated by extending existing drivers without rewriting code.

6. Testing & Debugging: Modular testing isolates issues and improves reliability.

### Conclusion

By leveraging both Open Source and Private Drivers with reusable modules, Octoffers efficiently automates job search and application processes across platforms.
