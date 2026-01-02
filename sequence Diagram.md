# Part 0 Diagrams
## Exercise 0.4 - New note
'''mermaid
sequence Diagram

    participant browser
    participant server

    browser->>server: User types not, clicks Save, not is sent
    server-->>browser: Note saved
    Note right of browser: Page updates to show the users note
'''

## 0.5: Single page app diagram
# In short all of the logig is on teh server, and the browser renders the HTML

'''mermaid

    participant browser
    pariticipant server

    browser->>server: GET /exampleapp/spa
    server->>browser: HTML file

    browser->>server: GET /exampleapp/spa.js
    server->>browser: JavaScript file

    Note of right browser: Browser runs JavaScript

    browser->>server: GET /exampleapp/data.json
    server->>browser: Notes as JSON

    Note of right browser: Browser renders notes on the page
    ,,,
