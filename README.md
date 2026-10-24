# @x12i/xentra-permissions usage example

Permission engine for Xentra.

This consuming application demonstrates **evaluate a scoped role grant and a missing permission** using the published npm package, pinned to `0.2.0`.

## Run

Requires Node.js 24 or newer and npm. The example needs no service credentials.

```sh
npm install --ignore-scripts
npm start
```

## Example

[`src/index.mjs`](src/index.mjs) contains the complete example. Assertions check the demonstrated behavior and the program prints a small result.

## When to use the package

- Evaluate whether a subject has permission for an operation.
- Reuse one permission engine across API and application entrypoints.

## Links

- [npm package](https://www.npmjs.com/package/@x12i/xentra-permissions)
- [Implementation monorepo](https://github.com/x12i/xentra)
- [Reviewed package source](https://github.com/x12i/xentra/tree/004372e6695509bf2e95d2e4e53d4534e81dd312/packages/permissions)

The `package.json` in this repository is private to prevent accidental publication of the example application under an npm package name.

## Local fixture scope

All identifiers, tokens, responses and records in this example are synthetic. Injected transports and in-memory stores do not contact a real identity provider, broker, VPN, or cloud service. File workflows create their own temporary directory and remove only that directory. The HTTP example binds a temporary loopback listener.
