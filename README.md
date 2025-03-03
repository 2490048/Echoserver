# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:

1. server

   import socket
HOST, PORT ='127.0.0.1', 65432
with socket.create_server((HOST, PORT)) as s:
    conn, addr = s.accept()
    with conn:
        print(f'Connected by {addr}')
        while data := conn.recv(1024):
            conn.sendall(data)

   2.clint

   import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'Rahul RP, 212224240125')
    print(f'Received: {s.recv(1024)!r}')


## OUTPUT:

1.server

![{D0D6E937-7BE0-4972-8586-4C17997062BB}](https://github.com/user-attachments/assets/67dcd1c6-061f-4438-8938-066ca00e0b39)

2.clint

![{FD3CC2A6-A993-412C-B37D-51F021FACF64}](https://github.com/user-attachments/assets/5ef2fbdc-9db9-4684-b5e8-3c940faefea4)



## RESULT:
The program is executed successfully
