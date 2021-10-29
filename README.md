# piping-server-pkg
[![CI](https://github.com/nwtgck/piping-server-pkg/actions/workflows/ci.yml/badge.svg)](https://github.com/nwtgck/piping-server-pkg/actions/workflows/ci.yml)

[Piping Server](https://github.com/nwtgck/piping-server) into an portable executable by [vercel/pkg](https://github.com/vercel/pkg) for Linux, macOS, Windows and Alpine

## Run on Linux

Run the command below, and a server runs on <http://localhost:8888>.

```bash
curl -L https://github.com/nwtgck/piping-server-pkg/releases/download/v1.7.0-4/piping-server-pkg-linuxstatic-x64.tar.gz | tar xzvf -
./piping-server-pkg-linuxstatic-x64/piping-server --http-port=8888
```

## Run on macOS

Run the command below, and a server runs on <http://localhost:8888>.

```bash
curl -L https://github.com/nwtgck/piping-server-pkg/releases/download/v1.7.0-4/piping-server-pkg-mac-x64.tar.gz | tar xzvf -
xattr -d com.apple.quarantine ./piping-server-pkg-mac-x64/piping-server
./piping-server-pkg-mac-x64/piping-server --http-port=8888
```

## Run on Windows

Download zip from <https://github.com/nwtgck/piping-server-pkg/releases/download/v1.7.0-4/piping-server-pkg-win-x64.zip>, extract it and run the command below, and a server runs on <http://localhost:8888>.

```ps1
.\piping-server.exe --http-port=8888
```

## Run on Alpine

Run the command below, and a server runs on <http://localhost:8888>.

```bash
curl -L https://github.com/nwtgck/piping-server-pkg/releases/download/v1.7.0-4/piping-server-pkg-alpine-x64.tar.gz | tar xzvf -
./piping-server-pkg-alpine-x64/piping-server --http-port=8888
```

## Run on Linux on ARM

Run the command below, and a server runs on <http://localhost:8888>.

```bash
curl -L https://github.com/nwtgck/piping-server-pkg/releases/download/v1.7.0-4/piping-server-pkg-linuxstatic-arm64.tar.gz | tar xzvf -
./piping-server-pkg-linuxstatic-arm64/piping-server --http-port=8888
```

Other built binaries found in <https://github.com/nwtgck/piping-server-pkg/releases> 

## Automation

These releases are automatically published by GitHub Actions.

## Generate executables in local

```bash
cd <this repo>
npm ci
npm run build-x64
```

```bash
cd <this repo>
npm ci
npm run build-arm64
```
