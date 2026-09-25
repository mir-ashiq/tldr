# kpsewhich

> Find the location of files in the TeX directory structure using kpathsea.
> More information: <https://manned.org/kpsewhich>.

- Show the full path of a file (e.g. a `.sty`, `.cls`, or `.tfm` file):

`kpsewhich {{filename}}`

- Search only files of a specific format (e.g. `tex`, `tfm`, `bst`, `otf`):

`kpsewhich -format={{fmt}} {{filename}}`

- Show all matching files, not only the first one:

`kpsewhich -all {{filename}}`

- Print the value of a TeX environment variable (e.g. `TEXMFHOME`):

`kpsewhich -var-value={{TEXMFHOME}}`

- Print the variable and brace expansion of a string:

`kpsewhich -expand-braces={{string}}`

- Print the search path used for a specific file format:

`kpsewhich -show-path={{fmt}}`

- Display version:

`kpsewhich -version`
