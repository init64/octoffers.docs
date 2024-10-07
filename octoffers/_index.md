---
title: "Octoffers"
weight: 1
---

Octoffers is a simple piece of software that can `fetch`, `export`, and `apply` available jobs on the different career
platforms. Commonly octoffers complete all these tasks using automated chrome-webdriver, but it dosen't mean that
Octoffers can't operate with a bare HTTP API. 

Each platform has its own `driver` which is compatible only with a
specific platform.

**Platform Driver** is an inherited class of a driver. 

Each platform driver includes at least the `apply` and `fetch` methods for the webdriver.
Each of these scripts preforms its task to complete its designated function. They might have diffrenet arguments representing various
additional features, such as *filter* or *coverletter*, but in the end, they share the same goal.

{{< button "./installation/" "Get started now" >}}
{{< button "https://alx.zolotarov.me/projects/octoffers/" "Read More" >}}
