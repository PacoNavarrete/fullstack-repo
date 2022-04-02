title New note (Halo from Mexico)

browser->server: HTTP POST /exampleapp/new_note
server-->browser: (status 302) URI has been changed temporarily to: /exampleapp/notes
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
server-->browser: HTML
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
server-->browser: main.js

note over browser:
In the 2 last lines of the main.js 
the browser executes the request 
to the server to get the data.json
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [[{"content":"jep","date":"2022-04-02T09:04:04.925Z"}, ...]

note over browser:
browser executes the 
xhttp.onreadystatechange = function ()
that renders notes to display
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/favicon.ico
server-->browser: HTML (favicon.ico)