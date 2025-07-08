sequenceDiagram
participant browser
participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>browser: Note saved successfully
    deactivate server

    Note right of browser: Browser updates the list of notes shown to the user
