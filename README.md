# Nelua LSP

This is an early implementation of writing an LSP server the for [nelua](https://nelua.io) programming language
It is heavily reliant on git to work but I aim to improve on this as much as I can

## Limitations

- I honestly do not properly know how to parse files, so anything that is read multiline will most likely not work
- Due to how I have to pass files to the compiler to mainitain each files context, there are multiple IO operations which makes the server very slow on larger files

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
    - Need to improve accuracy and handle more error cases
- [x] Completions (partial)
  - TODO:
    - Finish adding completions for stdlib
    - Completions for known variables and functions

## Dependencies
- [nelua](https://nelua.io)
- [cjson](https://github.com/DaveGamble/cJSON)
- [git](https://git-scm.com)

## How to Run
To use the current iteration, make sure you are in a local git repo

```sh
  nelua -L /path/to/nelua_lsp /path/to/nelua_lsp/main.nelua
```
