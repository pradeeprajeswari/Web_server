# Developing a Simple Webserver
NAME: PRADEEP.E
REFERENCE NUMBER: 23013416
DEPT: AIDS
# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using Python code

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
```
from http.server import HTTPServer, BaseHTTPRequestHandler

content= """
<html>
<head>
</head>
<body>
<h1>Welcome</h1>
</body>
</html>
"""

class HelloHandler(BaseHTTPRequestHandler) :
    def do_GET (self) :
        self.send response (200)
        self.send_header('Content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())


server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()
```
Type your code here
# OUTPUT:
![Alt text]![webserver1](https://github.com/pradeeprajeswari/Web_server/assets/145743112/2d47b1a3-174e-4393-9a48-e9be39f8c0e5)



# RESULT:

The program is executed succesfully
