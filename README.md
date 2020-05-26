# Stash Energy API Documentation

The documentation for the Stash Energy API uses the [OpenAPI 3 specification format](https://github.com/OAI/OpenAPI-Specification/).

Currently we use [ReDoc](https://github.com/Rebilly/ReDoc) to generate the HTML docs we host at <https://dev.stash.energy>

## How to view and/or edit the documentation

Prerequisites:

- node
- npm or yarn

### To view

1. `$ yarn build`
2. Open the generated redoc-static.html file in a web broswer

### To edit and see live changes while editing

1. `$ yarn dev`
2. Open a web browser at the URL specified in the command output
3. Make changes to the spec and save it
4. Refresh the web page to see the updated docs
