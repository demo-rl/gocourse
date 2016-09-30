#install git follow the install guide on 
https://git-scm.com/download/linux

# install mercurial 
https://www.mercurial-scm.org/downloads



# install go follow the install guide on
https://golang.org/doc/install


# Set up your go workspace

mkdir ~/gocourse
cd ~/gocourse
mkdir src pkg bin

# Put a reference of the GOPATH to yoour environment
export GOPATH=~/gocourse



# add go imports tool
go get golang.org/x/tools/cmd/goimports


# test the installation
mkdir -p  $GOPATH/src/github.com/user/hello

cat > $GOPATH/src/github.com/user/hello/hello.go <<EOF
package main

import "fmt"

func main() {
    fmt.Printf("hello, world\n")
}
EOF
