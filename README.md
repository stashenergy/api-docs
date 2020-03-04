# Stash Energy API Documentation

The documentation for the Stash Energy API uses the [OpenAPI 3 specification format](https://github.com/OAI/OpenAPI-Specification/).

Currently we use [ReDoc](https://github.com/Rebilly/ReDoc) to display the document on our [website](https://dev.stash.energy).

## How to view and/or edit the documentation

### Method 1: Swagger Editor

Open the [Swagger Editor](https://editor.swagger.io/) and either import the file, or paste the file contents in the editor. The Swagger Editor has a built-in validator that validates the schema and displays any errors. The preview is useful in visually detecting any issues, however it does not represent how the HTML docs will look because we use ReDoc to generate the HTML.

### Method 2: redoc-cli

Prerequisites:

- Node
- npx

#### To view

1. Run `npx redoc-cli bundle path/to/openapi.yaml`
2. Open the generated redoc-static.html file in a web broswer

#### To edit and see live changes while editing

1. Run `npx redoc-cli serve openapi.yaml --watch`
2. Open a web browser to the specified URL
3. Make changes to the spec and save
4. The html will automatically be regenerated
5. Refresh the web page to see updated docs

**Optionally:** Install redoc-cli globally and use the command directly:

1. `yarn global add redoc-cli` (or `npm -g install redoc-cli`)
2. `redoc-cli bundle/serve`
