# bitsadmin

> Manage the Background Intelligent Transfer Service (BITS).
> More information: <https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/bitsadmin>.

- Download a file using a single one-shot transfer job:

`bitsadmin /transfer {{job_name}} {{https://example.com/file.zip}} {{C:\path\to\file.zip}}`

- Create a download job and add a file to it:

`bitsadmin /create {{job_name}} && bitsadmin /addfile {{job_name}} {{https://example.com/file.zip}} {{C:\path\to\file.zip}}`

- Start a job, then finalize it once it has transferred:

`bitsadmin /resume {{job_name}} && bitsadmin /complete {{job_name}}`

- List the current user's transfer jobs with detailed information:

`bitsadmin /list /verbose`

- Cancel a job and remove it from the transfer queue:

`bitsadmin /cancel {{job_name}}`

- Continuously monitor transfer jobs (refresh every 5 seconds by default):

`bitsadmin /monitor`
