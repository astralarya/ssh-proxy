# ssh-proxy

**ssh-proxy** - Start a SOCKS proxy using an SSH connection on localhost (default port 9999)

## Installation

Add `ssh-proxy` to your PATH.

## Usage

**ssh-proxy** *CONNECTION* *[PORT]* *[OPTION...]*

Options
* __-\*__ : forward option to SSH (see `man ssh`)
* __-h__ : Show help

## Examples

Create a proxy via `user@example.com` on port 9999

    ssh-proxy user@example.com

Create a proxy via `user@example.com:5555` on port 1234

    ssh-proxy user@example.com:5555 1234

Create a proxy to the [named ssh connection](http://www.openbsd.org/cgi-bin/man.cgi/OpenBSD-current/man5/ssh_config.5?query=ssh_config&sec=5) `example` on port 9999

    ssh-proxy example
