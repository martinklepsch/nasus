Like Python's `SimpleHTTPServer` but scalable. Сan easily handle thousands of simultaneous connections.

Implemented with `Aleph` and `Netty` mostly as an example. It's still skillful and handy tho'. There's even nothing wrong with putting it to production.

## Usage

Run in the directory you want to serve:

```shell
clj -Sdeps '{:mvn/version {"nasus" "0.1.0"}}' -m http.server
```

## Features

* Plain text & HTML directory listings based on "Accept" header
* Automatic mime-type detection
* Streaming and chunked encoding for large files
* Keep-alive and slow requests handling
* Transperent content compression (gzip, deflate)

In development:

* Conditional requests: "ETag", "If-None-Match" and "Last-Modified"
* Range queries support
* SSL/TLS
* List of files & directories to exclude from serving

## Flags

TBD

## License

Copyright © 2019 Nasus

Nasus is licensed under the MIT license, available at MIT and also in the LICENSE file.