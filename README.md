# ToyLang -> WASM Compiler

## Prereqs

* .NET 9 SDK
* Node 18+ + Pnpm
* wasi-sdk/wasm-tools

Make sure `dotnet`, `npm`, `pnpm`, `nodemon` and `wasm-validate` are on your `$PATH`.

## Auto-tests

```bash
make install
make test
```

## Manual tests

```bash
make install
make cli compiler/tests/donut.toy
make cli compiler/tests/os.toy
# ...
```

## Starting the web UI

```bash
make install
make build
make start
```

Open http://localhost:3000.

## Style

* C#: `dotnet format` with the default style.
* TS/JS: prettier via `npx prettier . --fix`.
