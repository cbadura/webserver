# webserver
Our own implementation of an Nginx style server in C++, together with chltam and MrMOlten.
We used the socket API from C and poll() to listen on multiple ports to receive requests from a client.
Requests are parsed and responses are sent back accordingly, building the HTTP header and body.
Depending on request and endpoint, this process may be going through a CGI – both PHP and Python CGIs are working.

You can make GET, POST, and DELETE requests.
To change the default config, just edit the file (e.g. set auto index on and off, set the body size for POST requests, etc.)

## Installation

make

## Usage

./webserv \[ config file if you have one, without argument the default config will be loaded ]

Use curl or your web browser with localhost:PORT (default is 8080) to see the index page.
Check out the /files directory to see what we prepared
-> e.g., localhost:8080/upload.html lets you upload files. You can delete them or download them again.

![image](https://github.com/cbadura/webserver/assets/93912698/5bf51b46-2c4f-42f6-9eaf-902397fdd741)

