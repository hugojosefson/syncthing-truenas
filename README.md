# syncthing-truenas

Automatically downloading, then running
[syncthing](https://github.com/syncthing/syncthing) on an immutable TrueNAS
SCALE system.

## Install

### Pre-requisites

- A TrueNAS SCALE system, or other system where it's hard to install software
  directly.
- A user account on the system, logged in to a Linux terminal.
- A mounted filesystem where your user can write files, and execute them.

### Installation

Go to the directory where you have write access, and download the repo:

```bash
mkdir -p syncthing-truenas

curl -sfLS https://github.com/hugojosefson/syncthing-truenas/archive/refs/heads/main.tar.gz \
| tar xvz --strip-components=1 -C syncthing-truenas
```

## Usage

Then, go into the directory, and run the script to download and run syncthing as
the current user:

```bash
cd syncthing-truenas
./syncthing
```
