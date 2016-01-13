water-cooler
================
test
Super simple application leveraging `socket.io` and `express` that allows users to POST to an API and all browsers with the page open will have the text spoken out loud. Built to enable ChatOps.

## Running locally:
### Clone
``` git clone https://github.com/udryan10/water-cooler.git && npm install ```
### Run
``` sudo node server.js ```

## Deploying:
### Helper Script
``` ./deploy.sh ```
### Manually
``` docker run -d --name "water-cooler" -p 80:80 udryan10/water-cooler ```

## API Request
```curl -XPOST -H 'Content-Type: text/plain' -H 'X-Voice: Junior' http://localhost:8000/ -d 'this is my message'```
