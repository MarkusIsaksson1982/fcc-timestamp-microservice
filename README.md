# Timestamp Microservice

My solution to freeCodeCamp's [Build a Timestamp Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis-v9/lab-timestamp-microservice/lab-timestamp-microservice) lab (Back End Development and APIs). Node.js + Express 5, ES modules.

## API

| Request | Response |
|---|---|
| `GET /api/2015-12-25` | `{"unix":1451001600000,"utc":"Fri, 25 Dec 2015 00:00:00 GMT"}` |
| `GET /api/1451001600000` | same as above (Unix milliseconds) |
| `GET /api` | the current time |
| `GET /api/not-a-date` | `{"error":"Invalid Date"}` |

Date strings without a timezone are read as UTC, so results don't depend on the server's local timezone.

## Run

```bash
npm install
npm start   # http://localhost:8000
```
