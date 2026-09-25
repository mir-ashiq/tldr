# pdisk

> Menu-driven editor for Apple partition scheme disk partition tables.
> More information: <https://keith.github.io/xcode-man-pages/pdisk.8.html>.

- List partition tables for all available drives:

`pdisk -l`

- List the partition table of a specific disk:

`pdisk -l {{/dev/disk0}}`

- Interactively edit the partition table of a disk:

`pdisk {{/dev/disk0}}`

- Interactively edit the partition map without writing any changes to the disk:

`pdisk -r {{/dev/disk0}}`
