I have tried to make example given in document: http://golang.org/doc/talks/io2011/Writing_Web_Apps_in_Go.pdf with a current version of Go (at this time 1.0.2).

While following the document, I have encountered several obstacles in attempt to make examples working. It took me some time to figure out what changes to make, which libraries and functions to use. Examples given here are working on OSX installation. Would like to learn if they are working on lin/win too. 

Examples published here could be useful for someone who is exploring Go language, attempting to write standalone web server in Go. I have not found much examples around.

Files:

- ws.go - simplest possible web server in go
- ws_u.go - more developed example with error handling and file upload

ws_u uses provided .html files.

Usage:

    go run ws.go

or

    go run ws_u.go

(note that file upload example assumes uploading an image file jpeg, png, gif - whatever your browser will recognize as "image" mime)

when server is running: point your browser to http://localhost:8080

you may also compile examples to standalone executable:

    go build

shall compile all examples to binaries

    go build ws.go

shall compile only ws.go

on mac/unix you'd execute it as:

  ./ws

I assume that on windows 'go build ws.go' would create ws.exe

