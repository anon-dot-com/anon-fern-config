# Anon Fern Configuration

This repository contains your Fern configuration: 
  - [OpenAPI Spec](./fern/openapi/openapi.yaml)
  - [OpenAPI Overrides](./fern/openapi/openapi-overrides.yml)
  - [SDK generator config](./fern/generators.yml)

## Validating your OpenAPI spec

To validate your API, run: 
```sh
npm install -g fern-api # only required once
fern check
```

## Updating your SDKs

To update your SDKs, simply run the `Release TypeScript SDK` GitHub Action with the desired version for the release. Under the hood, this leverages the Fern CLI: 

```sh
npm install -g fern-api # only required once
fern generate --group ts-sdk
```