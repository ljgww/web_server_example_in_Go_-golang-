I have tried to make example given in document http://golang.org/doc/talks/io2011/Writing_Web_Apps_in_Go.pdf with a current version of Go (currently 1.0.2) and figured out that things from the example are not fully working in current version. It took me some time to make them working, so someone could find them useful as starters if writing web servers in Go

- ws.go - simplest possible web server in go
- ws_u.go - more developed example with error handling and file upload

Usage:

go run ws.go

or

go run ws_u.go

(note that file upload example assumes uploading an image file jpeg, png, gif - whatever your browser will recognize as "image" mime)

when server is running: point your browser to http://localhost:8080

