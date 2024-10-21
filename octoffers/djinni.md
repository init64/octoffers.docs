---
title: "Djinni"
weight: 1
---

Djinni was an easy platform to automate. You can run it in **headless mode** without any problems. 
The platform itself is very local and doesn't have many jobs available. 
The platform's lack of popularity means that competition is not as high as on some other large platforms. 

### Core Methods

**fetch**

Pretty standard implemention with only few exclusive features.

1. You can exclude key words from the search. 
2. AI Generated Cover letters. *(disabled at this moment)*

```python
    def fetch(
        self,
        role=None,
        tools=None,
        min_salary=None,
        exclusion_words: tuple = None,
        pages: int = 1,
    ):
```

Default webdriver arguments:

```python
self.chrome_args = ("--headless", "--no-sandbox", "--disable-dev-shm-usage")
```

