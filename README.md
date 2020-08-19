Go Generic tests
=================

This repository contains my tests with go generics.

- [Go Generic tests](#go-generic-tests)
  - [Quick execution](#quick-execution)
  - [go2go execution](#go2go-execution)
    - [Install go2go](#install-go2go)
    - [Run go2go](#run-go2go)
  - [License](#license)

Quick execution
---------------

Copy and paste the contents of the .go2 file to <https://go2goplay.golang.org/>
and click `Run`.

go2go execution
---------------

Installation and execution is the same as described on [Bill Kennedy's generics examples](https://github.com/ardanlabs/gotraining/blob/master/topics/go/generics/README.md)

### Install go2go ###

```sh
# Clone the current source code for Go on disk.
cd $HOME
mkdir go2go
cd go2go
git clone https://go.googlesource.com/go goroot
cd goroot

# Fetch all the branches and checkout dev.go2go.
git fetch
git checkout dev.go2go

# Change into the source directory and build.
cd src
./make.bash

# Navigate back to where you cloned the repo.
cd $GOPATH/github.com/massahud/gogenerics

# Then source the `.env` file located in the generics folder.
# export GO2GO_DEST=$HOME/go2go/goroot
# export PATH="$GO2GO_DEST/bin:$PATH"
# export GOROOT="$GO2GO_DEST"
# export GO2PATH="$GO2GO_DEST/src/cmd/go2go/testdata/go2path"
source .env

# With those settings in your current environment use this version of Go.
go version
# go version devel +2faeebf4e5 Tue Jun 23 04:54:48 2020 +0000 darwin/amd64
```

### Run go2go ###

```sh
go tool go2go run file.go2
```

License
-------

```text
Copyright 2020, Geraldo Augusto Massahud Rodrigues dos Santos

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
