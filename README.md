# GW (Go Watcher)

## Stacks

- Built in Go

## Features

A Wrapper of a command to watch any changes in filesystem, then re-run the command again.

## How to install

### Homebrew

```shell
$ brew install mattdamon108/tools/gw
```

### Using `go get`

```shell
$ go get -u github.com/mattdamon108/gw
```

### Build with the source code

1. Git clone

```shell
$ git clone https://github.com/mattdamon108/gw.git
```

2. Build & Install

```shell
$ go install
```

## How to use

```shell
$ gw [COMMAND arg1, arg2, ...]
```

e.g.

```shell
$ gw go run server.go
** Ctrl-C to exit **
2019/05/12 00:01:00 Listening to the port 8080...

# any changes in filesystem
Tyring to run the command...
2019/05/12 00:01:10 Listening to the port 8080...
```

- node.js
  You can use gw instead of nodemon.

```shell
$ gw node server.js
** Ctrl-C to exit **
Listening to port 4000

# any changes in filesystem
Tyring to run the command...
Listening to port 4000
```

## Next to do

- [ ] error handling
- [ ] reduce unnecessary re-runs
