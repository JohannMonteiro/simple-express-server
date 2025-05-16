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

## Dependencies
------------

* [ExpressJS](https://expressjs.com/)
* [dotenv](https://www.npmjs.com/package/dotenv)
* [nodemon](https://www.npmjs.com/package/nodemon)
