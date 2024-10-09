# Nelua LSP

This is an early implementation of writing an LSP server the for [nelua](https://nelua.io/) programming language
It is heavily reliant on git to work but I aim to improve on this as much as I can

## Goals

- [x] Go to Definition (partial)
  - TODO:
    - Proper matching for function parameters
    - No matching for comments and strings
- [ ] Hover
- [ ] Completions
- [ ] Diagnostics

## Dependencies
- [cjson](https://github.com/DaveGamble/cJSON)
- [git](https://git-scm.com/)

## How to Run
To use the current iteration, make sure you are in a git directory

```sh
  nelua -L /path/to/nelua_lsp /path/to/nelua_lsp/main.nelua
```
