```mermaid
sequenceDiagram
    participant browser
    participant server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server

    Note left of server: Responses only with 201 status code
    
    Note right of browser: Browser (JS) adds my message to message list without reloading
```