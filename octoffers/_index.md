---
title: "Octoffers"
weight: 1
---

Octoffers is a tool that can `fetch`, `export`, and `apply` for jobs in different career platforms using automated Chrome WebDriver{Selenium}, or in some cases, a bare HTTP API.

- Each platform has its own `driver` which is compatible only with a
specific platform.

- Platform Driver is an inherited class of a driver, including at least the `apply` and `fetch` methods.

These scripts act based on specific functions, with optional arguments like `filter or cover letter`, aiming to ease job applications.

Additional Features of Octoffers:

- **Customizations:** Users can specify filters like `job title`, `salary`, and `skills` for targeted job searches.
  
- **Session Management:** Handles user login sessions to allow easy application submissions without repeated logins.

- **Multi-Platform Support:** Interacts with multiple job portals through different platform drivers.

{{< button "./installation/" "Get started now" >}}
{{< button "https://alx.zolotarov.me/projects/octoffers/" "Read More" >}}
