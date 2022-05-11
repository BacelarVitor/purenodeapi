# PURENODEAPI

## A RESTful API for an uptime monitoring application

A RESTful API for an uptime monitoring application build from scratch using node without any framework or npm modules.

> An *"uptime monitor"* allows users to enter URLs they want monitored and receive alerts when those resources *"go down"* or *"come back up"*
> 

## Features

- [ ]  user sign-up
- [ ]  user sign-in
- [ ]  check URL's
- [ ]  send SMS alerts

## What we want the system to do (Backend spec)

1. The API listens on a PORT and accepts incoming HTTP requests for POST, GET, PUT, DELETE and HEAD
2. The API allows a client to connect, then create a new user, then edit and delete that user.
3. The API allows a user to *"sign in"* which gives them a token that they can use for subsequent authenticated requests.
4. The API allows the user to *"sign out"* which invalidates their token
5. The API allows a signed-in user to use then token to create a new *"check"*.
6. The API allows a signed-in user to edit or delete any of their checks.
7. In the background, workers perform all the "checks" at the appropriate times, and send alerts to the users when a check changes its state from *"up"* to *"down"*, or visa versa.

## Notes

[Twilio](https://www.twilio.com/go/twilio-brand-sales-pt-1?utm_source=google&utm_medium=cpc&utm_term=twilio&utm_campaign=G_S_LATAM_Brand_Twilio_Portuguese&cq_plac=&cq_net=g&cq_pos=&cq_med=&cq_plt=gp&gclid=CjwKCAjwve2TBhByEiwAaktM1Mn5jDOApoH1FV0osvmuUuAhM41Ay_2fyZ0rASYh3xgiIHrO7orOiBoCuqIQAvD_BwE) will be used for sending the SMS's
The data will be saved to the filesystem saved as JSON
The workers should run each 1 minute passed.

## Next steps

- [ ]  save the data to [firebase cloud store](https://firebase.google.com)
- [ ]  send e-mail
- [ ]  add tests
- [ ]  implement repository
- [ ]  implement clean architecture
- [ ]  recover password
- [ ]  welcome e-mail
- [ ]  confirm account e-mail
