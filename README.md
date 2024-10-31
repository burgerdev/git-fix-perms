# `git fix-perms`

This program aligns the permissions of files in the worktree with the permissions recorded in the index.
The primary use case is to retroactively fix the effect of an undesired `umask` during checkout.

## Installation

Copy (or link) the `git-fix-perms` executable to your `PATH`. E.g:

```sh
mkdir -p "$HOME/.local/bin"
ln -s "$PWD/git-fix-perms" "$HOME/.local/bin"
export PATH="$HOME/.local/bin:$PATH"
```

## Usage

```data
git fix-perms [-v|--verbose] [--dry-run]
```

Running the command without arguments aligns permissions of all files in the current worktree subdirectory.


