sequenceDiagram 

browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
activate server
server-->>browser: HTML code. HTTP Status Code - 200
deactivate server

browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
activate server
server-->>browser: The Javascript code. HTTP Status Code - 200
deactivate server

browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
activate server
server-->>browser: CSS code. HTTP Status Code - 200
deactivate server

browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/new_note_spa
activate server
server-->>browser: Return the notes as JSON data. HTTP Status Code - 200
deactivate server

Note right of browser: The server returns the webpage, Javascript code & the existing notes.
