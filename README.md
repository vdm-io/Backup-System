# Backup System for server:

The Bash scripts used to backup database and folders on a server

## Features

* Cross platform
* Fast and effective backups
* Backup to Dropbox
* Ability to track changes
* Historical records
* Preserve the folder structure
* Recourse friendly

## Getting started

Clone Repository

```bash
   $ git clone https://github.com/vdm-io/Backup-System.git Backup-System
```

Make sure the run file is executable

```bash
   $ cd Backup-System/
   $ chmod +x run.sh
```

## Auto Setup Option

Just run :)

```bash
   $ ./run.sh
```

## Manual Setup Option

Copy __config.txt__ to __config.sh__ and update the values in the file.

```bash
   $ cp config.txt config.sh
```

Copy __folders.txt__ to __folders__ and update the values in the file.

```bash
   $ cp folders.txt folders
```

Copy __databases.txt__ to __databases__ and update the values in the file.

```bash
   $ cp databases.txt databases
```

Run the script

```bash
   $ ./run.sh
```

## Fetch Backup and Restore

Either revert to previous backup (restore) or to do a new deployment.

```bash
   $ ./run.sh -r
```

## Tested Environments

* GNU Linux

If you have successfully tested this script on others systems or platforms please let me know!

## Running as cron job
Get the full path to the __run.sh__ file. Open https://crontab.guru to get your cron time settings. Open the crontab:
```bash
   $ crontab -e
```
With your cron time, add the following line to the crontab, using your path details:
> 5 03 * * * /path/to/run.sh >/dev/null 2>&1

> your time |  your path    | to ignore messages
   
## GIT, BASH

**Debian & Ubuntu Linux:**
```bash
    $ sudo apt-get install bash (Probably BASH is already installed on your system)
    $ sudo apt-get install git
```

**To use the Dropbox back-up option You also need the [Dropbox-Uploader](https://github.com/andreafabrizi/Dropbox-Uploader):**
```bash
    $ git clone https://github.com/andreafabrizi/Dropbox-Uploader.git Dropbox-Uploader
    $ cd Dropbox-Uploader/
    $ chmod +x dropbox_uploader.sh
    $ ./dropbox_uploader.sh
```

# Copyright:

* Copyright (C) [Vast Development Method](https://www.vdm.io). All rights reserved. 
* Distributed under the GNU General Public License version 2 or later
* See [License details](https://www.vdm.io/gnu-gpl)

