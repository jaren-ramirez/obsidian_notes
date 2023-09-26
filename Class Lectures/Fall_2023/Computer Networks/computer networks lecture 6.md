---
tags:
  - computer_science
  - networks
  - lecture
title: computer networks lecture 6
Lecturer: Dr. Pradeenban Kathiravelu
Class Number: CSCE A365
---
[[Computer Networks]]
```dataviewjs

```
```dataviewjs
let page = dv.current().file;
let creationTime = page.ctime;
let formattedDate = new Date(creationTime).toLocaleDateString();
dv.el("p", 'Created on ' + formattedDate)
```
# [[Socket]] Programming

## Important Links and Slides

[slides](data/slides/CSCE_A365_6.pptx)
## Outline

- Sub-Point
- Sub-Point
## Goals

- Clear understanding of [topic]
- Ability to explain [concept]
- Mastery of [skill/tool]
## Notes

- Two socket types
	- [[Udp]] 
	- [[Tcp]]
- [[Udp]]
	- no connection between client and server
	- no handshaking
	- sender explicity attaches IP destination address and port # to each packet
	- reciever extracts sender ip address and port # from recieved packet
	- transmitted data may be lost or recieved out of order
	- [[Datagrams]]
```jupyter
import socket
# AF_INET indicateds IPv4 addresses can be used
# SOCK_DGRAM with connectionless sevice for datagrams
server_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
# where we want to send the data
server_address = ('localhost',8001)
# bind it to the socket
server_socket.bind(server_address)
print("UDP server is waiting for incoming connections...")
while True:
	# Recieve data from the client, up to a maximum of 1024 byte (1kb)
	data, client_address = server_socket.recvfrom(1024)

	# Decode the received data, format with the variables involved, and display the string
	print(f"Received data from {client_address}: {data.decode()}")

	# create an acknowledgement
	ack = "Hey, this is the server acknowledging the reciept of your data: " + data.decode()

	# Encode the ackknowledgement and send to client
	server_socket.sendto(ack.encode(), client_address)
```


## Questions and Clarifications

## Summary





