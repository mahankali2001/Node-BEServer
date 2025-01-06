# NodeJSApp

# Install following node modules
- npm install express
- npm install -g nodemon
- npm install morgan
- npm install morgan-json
- npm install winston
- npm install cors
- npm install express-rate-limit
- npm install useragent

# What you learn in this project
- Express web framework
- Using different middlewares - global or applicaiton level, built-in, router level, error handling level, third party level
    - app middlewares - global logging, auth
    - built-in middlewares - Parse JSON or URL-encoded payloads
    - router middlewares - auth / authorization, request validation, rate limiting
    - error handling middlewares - central error handling, logging, provide user-friendly error pages,Logging to file
    - third party level - cors

- Error handling 
    - Use centralized location for Logs and Error Alerting - use structured logging to print errors in a formatted way and send them for safekeeping to a central location, like Sematext Logs, our log management tool.
    - 2 categories of errors to be handled
        - Operational errors - Use Custom Errors to Handle
            - Like, server connection failure, failed to resolve hostname, invalid user input, request timeout, 500 response, socket hang-up, out of memory
        - Programmer errors
            - These errors can often cause issues in your apps like memory leaks and high CPU usage. The best thing to do is to crash the app and restart it gracefully by using the Node.js cluster mode or a tool like PM2
            - Like, passing string Vs object / incorrect parameter in a fn, didn't resolve or catch rejected promise, calling async fn without a callback

# Reference - https://roadmap.sh/nodejs