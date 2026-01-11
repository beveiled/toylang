# ToyLang

![academic project](https://img.shields.io/badge/academic%20project-3DB420)
![source only](https://img.shields.io/badge/source%20only-545454)

> Handmade WASM compiler for the invented object-oriented language built with C# 

![Toylang](https://github.com/user-attachments/assets/cda4f960-4d65-4b02-aef5-02df52d242a6)

## Prerequisites

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
