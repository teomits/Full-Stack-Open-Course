# Page Load Diagram for /new_note_spa

```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: The user writes a note and clicks "Save"

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created (or success response)
    deactivate server

    Note right of browser: The browser updates the UI dynamically using JavaScript
```
