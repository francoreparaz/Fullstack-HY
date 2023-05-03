# Fullstack-HY
```mermaid
sequenceDiagram
    participant browser
    participant server
    
    browser->>server: POST  https://studies.cs.helsinki.fi/exampleapp/new_note
    browser->>server: GET   https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    server-->>browser: New List
    desactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: the css file
    desactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: the JavaScript file
    desactivate server
    

    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->> List 
    desactivate server    

    Note right of browser: The browser executes the callback function that renders the notes 
```
