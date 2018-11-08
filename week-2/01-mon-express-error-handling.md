# Warmup: Express Error Handling

* Read here: https://learn-2.galvanize.com/cohorts/757/blocks/29/content_files/Server%20Development/07-errors.md

* Look at Dan Levy's express guide app.js code here: https://github.com/justsml/guides/blob/master/express/setup-guide/app.js


## Questions:

* Why do we need error handling in an express app?
  - So that the developer & server knows what's going wrong if there's an error
  - So that we can inform the client/end user if something goes wrong
  - Why would something go wrong?
    * Our code could have a mistake
    * Client could try to use the server in a way it's not intended for
    * Someone could make requests to the server from places other than our designated client/front-end (Postman, Curl requests, etc.)
  - We don't want our server to crash if there's an error
    * We want to 'catch' the error and handle it appropriately
    
* What does the next function in an express route do?
  - Keeps things moving
  - Pass along an error from within a route if necessary
  
* What does res.status() do?
  - Sets HTTP status for your response
  - Choose any status code you want
  - Chainable
  
* Why do we need two error handling functions?
  - What does each one do?
    * 404 not found handler
      - Catch errors that happened when no route is matched
    * General error handler
      - Catch errors that have happened within the routes
      
* Why do they need to be at the bottom/after our routes?
  - Because of the order in which routes are processed/matched
  - Error handlers are last case/worst case scenario so they should be that last things that can match a request