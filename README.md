# Skills

This is a collection of skills that can be used to enhance the AI's capabilities or just to have a good laugh. These
skills are designed to be small and enjoyable, sometimes even useful.

## Compatibility

This repository is designed to be compatible with [npx skills](https://github.com/vercel-labs/skills) and should work
with any Agent that supports the open standard.

## Installation

You can install the skills by running the following command:

```
npx skills add https://github.com/theholocoder/skills
```

Or you can install only specific skills by running the following command:

```
npx skills add https://github.com/theholocoder/skills --skill yoda
```

## Skills available

### ASCII-This

Renders text as ASCII art block letters, draws ASCII diagrams (boxes, arrows, system interactions, flowcharts, sequence
diagrams), or produces freehand ASCII drawings of any subject (animals, objects, scenes, characters). Three modes are
automatically selected based on the request: text art, diagram, or freehand drawing.

Install it with:

```
npx skills add https://github.com/theholocoder/skills --skill ascii-this
```

#### Example

> make a diagram of an HTTP request from the browser to the webserver

```text
.-------------.          +-------------------+          +================+
|    User     |          |   Web Browser     |          ||    Server    ||
|  (You)      |          |                   |          ||  (Apache /   ||
'-------------'          +-------------------+          ||   Nginx)     ||
       |                          |                     +================+
       |   [clicks a link /       |                            |
       |    types a URL]          |                            |
       |------------------------->|                            |
       |                          |                            |
       |                          |  [1: TCP Handshake SYN]   |
       |                          |--------------------------->|
       |                          |  [2: TCP Handshake SYN-ACK]
       |                          |<---------------------------|
       |                          |  [3: TCP Handshake ACK]   |
       |                          |--------------------------->|
       |                          |                            |
       |                          |  [4: HTTP GET /index.html] |
       |                          |  Host: example.com         |
       |                          |  Accept: text/html         |
       |                          |  User-Agent: Mozilla/5.0   |
       |                          |--------------------------->|
       |                          |                            |
       |                          |                     [5: server processes
       |                          |                      request, reads file]
       |                          |                            |
       |                          |  [6: HTTP 200 OK]          |
       |                          |  Content-Type: text/html   |
       |                          |  Content-Length: 3452      |
       |                          |                            |
       |                          |  <html>...</html>          |
       |                          |<---------------------------|
       |                          |                            |
       |   [renders page]         |                            |
       |<-------------------------|                            |
       |                          |  [7: TCP FIN — close conn] |
       |                          |--------------------------->|
       |                          |<---------------------------|

```

### Yoda

Forces the LLM to communicate exclusively in Yoda's speech style from Star Wars: inverted syntax, archaic diction,
wisdom-laden phrasing.

## Licence

MIT
