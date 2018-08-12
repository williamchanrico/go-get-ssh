# go-get-ssh
Wrapper for "go get -v -u" using ssh git clone

## What it does
- The script will `git clone` (using your configured `ssh` credential) the repository into your workspace with the correct `go` structure (`$GOPATH/src/domain.com/repo_owner/repo_name/`).
- And it will run `go get -u -v` in the cloned repository.
- Done. It does everything you need to start building/developing that repo in one command.

## Usage
```
$ go-get-ssh
usage: go-get-ssh IMPORT_PATH
example:
         go-get-ssh github.com/tokopedia/gosample

         Will be imported to:
         $GOPATH/src/github.com/tokopedia/gosample
```
