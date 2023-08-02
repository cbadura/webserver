# webserver
Our own implementation of an Nginx style server in C++, together with chltam and MrMOlten
You can make GET, POST, and DELETE requests.
Php and python CGIs are working.
To change the default config, just edit the file (e.g. set auto index on and off, set the body size for POST requests, etc.)

Installation:

make

Usage:

./webserv \[ config file if you have one, without argument the default config will be loaded ]

Use curl or your web browser with localhost:PORT (default is 8080) to see the index page.
- localhost:8080/upload.html lets you upload files. You can delete them or download them again.
