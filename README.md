# go-template • [![CI](https://github.com/transmissions11/foundry-template/actions/workflows/tests.yml/badge.svg)](https://github.com/transmissions11/foundry-template/actions/workflows/tests.yml)

Template for getting started with a Go repository.

To get started, launch `go mod init github.com/<your-account>/<your-repo-url>`

## Build

Build for current OS with `go build`

Build for Linux from Windows with:
- `$Env:GOOS = "linux"; $Env:GOARCH = "amd64"`
- `go build`

## Release

before releasing, always update the version inside the CI/CD config file `.github/workflows/release.yaml` ("tag" field) to the release version of your choice.

To release a new version, simply merge into the main branch, the CI/CD will take care of creating a new tag and release on GitHub.