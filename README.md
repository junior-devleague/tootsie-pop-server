# Tootsie Pop Server

How many requests does it take to get to the "center" of your server? In this project, we will use networking basics and the HTTP protocol to build a simple server that sends data a browser can understand.

###Objective

Your server must accept and keep track of how many requests each client's IP has made, and on the client's 50th request, send them a special response.

###Prerequisites

- Basic understanding of and experience with networking beyond the browser (telnet, socket connections, etc.)
- Understand how an HTTP request is built and how to make one from within Python.

###Requirements

To complete this project you will need Python 3.0 or greater, a terminal, and a text editor.

###Desired Outcome

By the completion of this exercise, students should understand both the client and server side of the HTTP protocol, how to structure and use HTTP requests and responses programmatically, and know how a real web server gets content to its visitors.

###Your challenge
- Create a `client.py` and a `server.py`
- `client.py` must make a request to a machine on the local network in this room, and must display the response it receives to standard output.
- `server.py` must listen for requests on port 8080 and send HTTP responses to all clients that do so.
- `server.py` must send any client that has visited more than 50 times a special response of your choosing (can be a string, an HTML file, or redirecting them to an external site)

###Resources

- [`urllib` for Python](https://docs.python.org/3/library/urllib.html)
- [http.server module for Python](https://docs.python.org/3/library/http.server.html)
- [Requests library for Python](http://docs.python-requests.org/)

###Further goals

Once your server meets the objective, you can implement some basic cybersecurity by placing a limit on the rate of requests from an individual client. This limit must be able to differentiate between automated traffic and legitimate traffic--you don't want to block real people from seeing your secret message, but you don't want automated scripts eating all your resources.
