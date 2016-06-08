# handler/gzip

Gzip compression handler for golang.

## Features

* Transparent Compression
* White list of Content-Type prefixes, to decide what to compress
* Pooling of the GZip Writer
* Only compress, if the result is not already compressed

## usage

```
import "github.com/smancke/handler/gzip"
 ...
server := httptest.NewServer(NewGzipHandler(your_handler()))
``` 
