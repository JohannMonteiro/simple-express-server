# ExpressJS Server
====================

A simple server made with ExpressJS for managing tea data.

## Table of Contents
-----------------

* [Getting Started](#getting-started)
* [API Endpoints](#api-endpoints)
* [Dependencies](#dependencies)

## Getting Started
---------------

To run the server, follow these steps:

1. Clone the repository
2. Install dependencies using `npm install` or `yarn install`
3. Start the server using `npm start` or `yarn start`

## API Endpoints
--------------

The server provides the following API endpoints:

### POST /teas

Create a new tea entry

* Request Body: `{ name: string, price: number }`
* Response: `{ id: number, name: string, price: number }`

### GET /teas

Retrieve all tea entries

* Response: `[ { id: number, name: string, price: number } ]`

### GET /teas/:id

Retrieve a tea entry by ID

* Response: `{ id: number, name: string, price: number }`

### PUT /teas/:id

Update a tea entry by ID

* Request Body: `{ name: string, price: number }`
* Response: `{ id: number, name: string, price: number }`

### DELETE /teas/:id

Delete a tea entry by ID

## Logging
--------

The server uses a custom logging middleware to log incoming requests. The logger writes log messages to the console in the following format:

`:method :url :status :response-time ms`

For example:

`GET /teas 200 10ms`

The logger also uses the `winston` library to log messages at different levels (e.g., info, error). You can configure the logging level by modifying the `logger.js` file.


## Dependencies
------------

* [ExpressJS](https://expressjs.com/)
* [dotenv](https://www.npmjs.com/package/dotenv)
* [nodemon](https://www.npmjs.com/package/nodemon)
* [winston](https://www.npmjs.com/package/winston)
* [morgan](https://www.npmjs.com/package/morgan)
