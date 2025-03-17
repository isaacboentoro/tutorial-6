# Reflection Notes

## Reflection 1
The `handle_connection` function in the code processes incoming TCP connections from a web client. It takes a mutable TcpStream as input, representing the connection to a client. It creates a buffered reader around the stream for more efficient line by line reading, and reduces system calls. It then processes the HTTP request, reading the input stream liine by line, returning Result for each line and mapping each Result , continuing until it hits an empty line, and collects all lines into a vector. It then outputs the recieved HTTP request to the console using a pretty-print format.

