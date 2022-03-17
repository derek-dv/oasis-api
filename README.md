# OASIS API

This package is for client applications to connect and work with the OASIS API

- [OASIS API](#oasis-api)
  - [Getting started](#getting-started)
  - [Auth](#auth)
    - [Login](#login)
    - [Signup](#signup)

## Getting started

To get started with this package run

`npm install oasis-api`

This installs the package to your project.
To use it in the Application, it can be imported by

`import oasis from "oasis-api"`

## Auth

The Auth class handles the authentication of the oasis-api. It can be imported by:

`import { Auth } from "oasis-api"`

### Login

To login use this code:

` import { Auth } from "oasis-api"

const oasisAuth = new Auth()

const user = await oasisAuth.login({
email: "email@test.com",
password: "testpass"
})
`

### Signup

For signup, use this code snippet:

` import { Auth } from "oasis-api"

const oasisAuth = new Auth()

const data = await OasisAuth.signup({
firstName: 'test',
lastName: 'test',
email: 'test@email.com',
password: 'test',
confirmPassword: 'test',
acceptTerms: true,
avatarType: "User",
title: "Mr",
});
`
