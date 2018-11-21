# Warmup: Intro to JWTs

## Resources

* [Learn - Intro to JWTs](https://learn-2.galvanize.com/cohorts/757/blocks/29/content_files/Authentication%20and%20Authorization/05-jwt-intro.md)

## Questions

* What is a JWT (in your own words)?
  - JSON Web Token
  - Post-authentication: after you've been authenticated, server provides you with a token

* How do JWTs help us authorize users?
  - Gives you permission to do things on site/app
  - Gives you privelages based on your authentication
  - Temporary proof of who you are

* What kind of information should be stored in a JWT?
  - User:
    * **USER ID** (PRIMARY KEY)
  - Authorization that they have
  - Maybe when it was created

* Is the information contained in a JWT secure?
  - NOOOOO
  - NOT SECURE
  - **NO PASSWORDS!!!**