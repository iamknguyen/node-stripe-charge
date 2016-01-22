## Node + Stripe + Express

[![Build Status](https://travis-ci.org/mjhea0/node-stripe-charge.svg?branch=master)](https://travis-ci.org/mjhea0/node-stripe-charge)

[![Coverage Status](https://coveralls.io/repos/mjhea0/node-stripe-charge/badge.svg)](https://coveralls.io/r/mjhea0/node-stripe-charge)

[![npm version](https://badge.fury.io/js/node-stripe-charge.svg)](http://badge.fury.io/js/node-stripe-charge)

This is the back-end API, which includes:

1. User auth via JSON web tokens
1. Stripe integration
1. Testing via Mocha and Chai as well as Istanbul for code coverage

## Quick Start

1. Clone and install dependencies
1. Update the config:
  - Rename the *.env_sample* file to *.env* and update
  - Update the Mongo URI in */src/_config.js* (if necessary)
1. Run `mongod` in a seperate terminal window
1. Run the app - `npm start` or `gulp`

> The database, if empty, is seeded with an admin user - username: *ad@min.com* / password: *admin*

## Tests

Without code coverage:

```sh
$ gulp test
```

With code coverage:

```sh
$ npm cov
```

## API Documentation

### User

- GET `/users` - get all users
- GET `/user/:id` - get user
- POST `/users` - create user
- PUT `/user/:id` - update user
- DELETE `/user/:id` - delete user

### Auth

- POST `/auth/login` - login user

### Item

- GET `/items` - get all items
- GET `/item/:id` - get item
- POST `/items` - create item
- PUT `/item/:id` - update item
- DELETE `/item/:id` - delete item

### Store

- GET `/stores` - get all stores
- GET `/store/:id` - get store
- POST `/stores` - create store
- PUT `/store/:id` - update store
- DELETE `/store/:id` - delete store