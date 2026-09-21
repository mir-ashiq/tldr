# psd

> Symlink and sync browser profiles to RAM (tmpfs), reducing disk I/O.
> More information: <https://github.com/graysky2/profile-sync-daemon>.

- Preview what psd will do or is doing (profile sizes, paths, recovery snapshots):

`psd p`

- Delete all accumulated crash-recovery snapshots:

`psd c`

- Enable and start the daemon (also starts the hourly resync timer):

`systemctl --user enable --now psd.service`

- Restart the daemon to apply configuration file changes:

`systemctl --user restart psd.service`
