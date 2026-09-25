# mirrorselect

> Select fast Gentoo source and rsync mirrors, interactively or by automatic speed testing.
> More information: <https://wiki.gentoo.org/wiki/Mirrorselect>.

- Open the interactive mirror selection interface:

`sudo mirrorselect -i`

- Interactively select from the download mirrors of a specific country:

`sudo mirrorselect -i -c "{{United States (USA)}}"`

- Automatically select the 3 fastest download mirrors (deep test, 10 blocks per mirror):

`sudo mirrorselect -s3 -b10 -D`

- Interactively pick an rsync mirror and append the selection to the ebuild repository config:

`sudo mirrorselect -i -r -o >> /etc/portage/repos.conf/gentoo.conf`
