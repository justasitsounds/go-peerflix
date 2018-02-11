# Go Peerflix

A Golang port of [peerflix](https://github.com/mafintosh/peerflix).

<img src="https://api.travis-ci.org/Sioro-Neoku/go-peerflix.svg?branch=master" />

Start watching the movie while your torrent is still downloading!
![Working of go-peerflix](./images/demo.gif)

## Installation

Download the binary from the [releases](https://github.com/Sioro-Neoku/go-peerflix/releases) page.

Or in case you have golang configured you may want to build from source (requires dep for vendoring)

```sh
git clone https://github.com/Sioro-Neoku/go-peerflix
dep ensure
```

## Usage
Access the stream on [http://localhost:8080/](http://localhost:8080/)
```sh
go-peerflix [magnet url|torrent path|torrent url]
```

To start playing in VLC:
```sh
go-peerflix -player vlc [magnet url|torrent path|torrent url]
```

Currently supported players are: VLC, MPlayer, OMXPlayer and MPV

## Build

Building only for the current platform:

```bash
go build .
```


Building for platforms: Linux, Darwin and Windows

```bash
goxc
```


## License
[MIT](https://raw.githubusercontent.com/Sioro-Neoku/go-peerflix/master/LICENSE)
