# Stash Energy API Documentation

The documentation for the Stash Energy API uses the [OpenAPI 3 specification format](https://github.com/OAI/OpenAPI-Specification/).

Currently we use [ReDoc](https://github.com/Rebilly/ReDoc) to generate the HTML docs we host at <https://dev.stash.energy>

## How to view and/or edit the documentation

### redoc-cli

Prerequisites:

- npx

#### To view

1. `$ npx redoc-cli bundle path/to/openapi.yaml`
2. Open the generated redoc-static.html file in a web broswer

#### To edit and see live changes while editing

1. `$ npx redoc-cli serve path/to/openapi.yaml --watch`
2. Open a web browser at the URL specified in the command output
3. Make changes to the spec and save
4. The html will automatically be regenerated. Refresh the web page to see updated docs

**Optionally:** Install redoc-cli globally and use the command directly:

1. `$ yarn global add redoc-cli` (or `npm -g install redoc-cli`)
2. `$ redoc-cli ...`
