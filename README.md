# Nelua LSP

This is an early implementation of writing an LSP server the for [nelua](https://nelua.io/) programming language
It is heavily reliant on git to work but I aim to improve on this as much as I can

## Goals

- [x] Go to Definition (partial)
- [ ] Hover
- [ ] Completions
- [ ] Diagnostics

## Dependencies
- [cjson](https://github.com/DaveGamble/cJSON)
- [git](https://git-scm.com/)

## How to Run

```sh
  nelua -L /path/to/nelua_lsp /path/to/nelua_lsp/main.nelua
```
