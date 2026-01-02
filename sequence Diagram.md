'''mermaid
sequence Diagram

    participant browser
    participant server

    browser->>server: User types not, clicks Save, not is sent
    server-->>browser: Note saved
    Note right of browser: Page updates to show the users note
'''