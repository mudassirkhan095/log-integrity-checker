# Log Integrity Checker

A simple security tool that checks whether log files have been modified or tampered with by using SHA-256 cryptographic hashing.

## Features

- Accepts a single log file or a directory.
- Calculates SHA-256 hashes.
- Stores hashes for future integrity checks.
- Detects modified files through hash comparison.
- Reports possible file tampering.
- Allows authorized users to update stored hashes.

## Usage

Initialize hashes:

    ./integrity-check init /var/log

Check a log file:

    ./integrity-check check /var/log/syslog

Update the stored hash after an authorized change:

    ./integrity-check update /var/log/syslog

## Technology

- Bash
- SHA-256
- Linux
- File Integrity Monitoring

## Project URL

https://github.com/mudassirkhan095/log-integrity-checker
