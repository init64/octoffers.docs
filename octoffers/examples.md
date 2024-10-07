---
title: "Example use cases"
weight: 4
---

Djnni
------

**Fetch 5 pages (about 50 roles) via djinni**
```bash
python octoffers djinni fetch devops --pages 5
```
**Apply to all available jobs via djinni**
```bash
python octoffers djinni apply "Hello, I'm looking for job" # <-- Cover letter
```

Indeed
------
**Authorize platform driver**
```bash
python octoffers indeed login jhondoe@exmaple.org # <-- Email
```

**Fetch 100 pages via indeed**
```bash
python octoffers indeed fetch "devops" -p 100 -e -s # <-- Easy apply + Sorted by date 
```

**Apply to all avaiable jobs via indeed**
```bash
python octoffers indeed apply
```
