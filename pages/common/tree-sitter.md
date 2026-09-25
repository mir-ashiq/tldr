# tree-sitter

> Command-line tool for creating, testing, and using Tree-sitter parsers.
> More information: <https://github.com/tree-sitter/tree-sitter>.

- Generate a parser in C from the grammar in the current directory (`grammar.js`):

`tree-sitter generate`

- Parse files and report any errors (reads from `stdin` if no paths are given):

`tree-sitter parse {{path/to/file}}`

- Run the corpus test suite of the parser in the current directory:

`tree-sitter test`

- Run only the tests matching a `regex`, updating expected outputs where needed:

`tree-sitter test --include "{{test_name_pattern}}" --update`

- Run a query file against source files and show the matches:

`tree-sitter query {{path/to/query.scm}} {{path/to/file}}`

- Syntax-highlight a file with ANSI colors:

`tree-sitter highlight {{path/to/file}}`
