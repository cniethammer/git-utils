# git-utils
git-utils provides a collection of utilities and additional subcommands for daily git tasks

> **Note:** The tools currently support **Linux only**. They rely on GNU `getopt` (util-linux) for long options, which macOS and the BSDs do not provide.

| Tool | Description | Requirements |
|------|-------------|--------------|
| `git-clean-merged` | Delete merged local and remote branches | Git ≥ 2.23, Bash ≥ 4 |
| `git-make-tgz` | Archive a commit, tag or branch as `.tar.gz` | Git ≥ 2.25 |

## Getting Started

### Prerequisites
The tools are Bash scripts and need only Git and standard command-line tools (coreutils, grep).
The minimum versions are listed in the table above.

Both tools parse long options with GNU `getopt` (part of util-linux), which is preinstalled on most Linux distributions.
Other platforms are not supported: macOS, for example, ships a BSD `getopt` without long-option support and Bash 3.2 as `/bin/bash`.

### Installation
Clone the repository and make the scripts available on your `PATH` or call them via `git` from the clone directory.
No additional steps are required.

### Usage

To see the usage of the scripts, use the `--help` option.
With the scripts on your `PATH`, they can also be called as git subcommands, e.g. `git clean-merged --dry-run`.


## Legal Info and Contact
This software is published under the terms of the BSD license.
