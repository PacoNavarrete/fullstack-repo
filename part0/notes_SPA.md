title New note(SPA )

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa
server-->browser: HTML
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa.js

note over browser:
In the main.js 
the browser executes the request 
to the server to get the data.json
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{"content":"teste","date":"2022-04-02T12:31:41.287Z"} ...]

note over browser:
browser executes the 
var redrawNotes = function()
that renders notes to display
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/favicon.ico
server-->browser: HTML (favicon.ico)