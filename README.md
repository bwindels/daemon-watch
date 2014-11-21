# Daemon watch
A tool to run multiple daemons from the console, and to kill them all at once. Useful for situations where you have to run multiple tools in the background, like when setting up `make watch`.

## Usage

```
daemon-watch [cmd --name <name> [--cwd <cwd>]]*
```

## Description

Will run all the passed commands and forward their `stdout` and `stderr`, prepended with the given name. If you send `SIGINT` (with control + c) or `SIGTERM` to daemon-watch, it will forward the signals to all the commands it is running

##Installation

```
npm install daemon-watch
```
