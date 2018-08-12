# go-get-ssh
Wrapper for "go get -v -u" using ssh git clone

## What it does
- The script will `git clone` the repository into your workspace with the correct `go` structure (`$GOPATH/src/domain.com/repo_owner/repo_name/`)
- Run `go get -u -v` in the cloned repository
- Done. It does everything you need in to pull that repo in one commands and earns you more time to enjoy your coffee

## Usage
```
$ go-get-ssh
usage: go-get-ssh IMPORT_PATH
example:
         go-get-ssh github.com/tokopedia/gosample

         Will be imported to:
         $GOPATH/src/github.com/tokopedia/gosample
```
