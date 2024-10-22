# Nelua LSP

This is an early implementation of writing an LSP server the for [nelua](https://nelua.io) programming language
It is heavily reliant on git to work but I aim to improve on this as much as I can

## Disclaimer

I honestly do not properly know how to parse files so anything that be read multiline will most likely not work

## Goals

- [x] Go to Definition (partial)
  - TODO:
    - Proper matching for function parameters
    - No matching for comments and strings
- [x] Hover (partial)
  - TODO:
    - Check for multiple declarations with different types but same identifier
- [x] Diagnostics (partial)
  - TODO:
    - Diagnostics come in quite slowly
    - Diagnostics can be inconsistent
- [x] Completions (partial)
  - TODO:
    - Finish adding completions for stdlib
    - Completions for known identifiers

## Dependencies
- [nelua](https://nelua.io)
- [cjson](https://github.com/DaveGamble/cJSON)
- [git](https://git-scm.com)

## How to Run
To use the current iteration, make sure you are in a local git repo

```sh
  nelua -L /path/to/nelua_lsp /path/to/nelua_lsp/main.nelua
```
