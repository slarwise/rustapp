# Rust App

## Usage

To start the http server on port 3000, do

```sh
cargo run
```

To make a request, do

```sh
curl http://localhost:3000
```

To view the api documentation, do

```sh
npx @redocly/cli preview-docs openapi.yaml
```

and follow the instructions. This requires [npm](https://www.npmjs.com) to be
installed. To verify that the implementation follows the documentation, do

```sh
cargo run &
npx specmatic  test --testBaseURL=http://localhost:3000  openapi.yaml
```

This requires [specmatic](https://specmatic.in/getting_started.html) to be
installed.
