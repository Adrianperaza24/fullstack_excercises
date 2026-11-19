## 0.6 New note in Single page app diagram

```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 with 'message': 'note created'
    deactivate server

    Note right of browser: Now the browser only sends a single POST request and handles the rendering of the page in the browser.

  ```