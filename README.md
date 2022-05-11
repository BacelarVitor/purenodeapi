# purenodeapi

A RESTful API for an uptime monitoring application build from scratch using node without any framework or npm modules.

An _"uptime monitor"_ allows users to enter URLs they want monitored and receive alerts when those resources _"go down"_ or _"come back up"_

## Features

[] - user sign-up
[] - user sign-in
[] - check URL's
[] - send SMS alerts

## What we want the system to do (Backend spec)

1. The API listens on a PORT and accepts incoming HTTP requests for POST, GET, PUT, DELETE and HEAD
2. The API allows a client to connect, then create a new user, then edit and delete that user.
3. The API allows a user to _"sign in"_ which gives them a token that they can use for subsequent authenticated requests.
4. The API allows the user to _"sign out"_ which invalidates their token
5. The API allows a signed-in user to use thein token to create a new _"check"_.
6. The API allows a signed-in user to edit or delete any of their checks.
7. In teh background, workers perform all the "checks" at the appropriate times, and send alerts to the users when a check changes it's state from _"up"_ to _"down"_, or visa versa.

## Notes

Twilio will be used for sending the SMS's
The data will be saved to the filesystem saved as JSON
The workers should run each 1 minute passed.

## Next steps

[] - Save the data to Firebase db
[] - Send E-mail
[] - Add tests
[] - Implement Repository
[] - Implement Clean Architecture
[] - Recover password
