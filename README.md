## networking-fundamentals
##OSI MODEL

| ** OSI Layer**  || ** Nickname**  ||  ** Role Real-World Example ** 
----------------------------------------------------------------------------
| 7. Application	| The Pizza Orderer	| You use DoorDash to order a pizza. You don’t care how it arrives—you just click "Buy".
------------------------------------------------------------------------------------------------------------------------------
| 6. Presentation	| The Emoji Translator | Sending a meme that gets auto-converted to JPEG so your grandma’s flip phone can open it. 
------------------------------------------------------------------------------------------------------------------------------
| 5. Session	| The Bouncer | Starting a Zoom call, chatting, and ending it when someone says, "I gotta go water my plants".
------------------------------------------------------------------------------------------------------------------------------
| 4. Transport | The Delivery Guy | Splitting a TikTok video into chunks and ensuring none get lost (TCP: "Got it? Resend if not!").
------------------------------------------------------------------------------------------------------------------------------
| 3. Network | The GPS Navigator | Google Maps rerouting you around traffic to get to the concert on time.
------------------------------------------------------------------------------------------------------------------------------
| 2. Data Link | The Neighborhood Mailman | Your Wi-Fi router sends Netflix data to your laptop, not your roommate’s phone.
------------------------------------------------------------------------------------------------------------------------------
| 1. Physical | The Highway | The Ethernet cable or Wi-Fi signal carries data like road cars. Bonus drama: "Why is the Wi-Fi so slow?!"
------------------------------------------------------------------------------------------------------------------------------


In Summary: 1. Order it (Application ) → 2. Translate your order to emojis (Presentation ) → 3. Confirm the order (Session ) → 4. Split the pizza into slices (Transport ) → 5. Find your address (Network ) → 6. Deliver to YOUR door (Data Link ) → 7. Pizza arrives via bike/car (Physical).

## Subnetting Calculation

## Subnetting divides a large network into smaller, manageable subnetworks. Below is a calculation example for an IP range: (I used https://subnettingpractice.com/subnet-calculator.html for my calculation)

IP Address: 41.76.82.198
-------------------------

Network Address: 41.76.82.0
-------------------------

Broadcast: 	41.76.82.255
-------------------------

Subnet Mask: 255.255.255.0
-------------------------

Slash: /24
-------------------------

First Usable Host: 41.76.82.1
-------------------------

Last Usable Host: 41.76.82.254
-------------------------

Usable Hosts: 254 
-------------------------

![image](https://github.com/user-attachments/assets/47bb4d99-aeb9-4256-920c-85f97cbab1e8)


## TCP/IP Protocol Suite in Action

Scenario: Loading a webpage (e.g., https://example.com).

Process:

1. Application Layer (HTTP/HTTPS):

    The browser sends an HTTP GET request.

    DNS resolves example.com to an IP (e.g., 93.184.216.34).

2. Transport Layer (TCP):

     TCP performs a three-way handshake (SYN > SYN-ACK > ACK) to establish a connection.

      Data is segmented and reassembled with error-checking.

3. Internet Layer (IP):

    IP routes packets between your device and the server using the destination IP.

    Routers update the packet’s TTL and forward it.

4. Link Layer (Ethernet/Wi-Fi):

     Frames are sent using MAC addresses between local devices (e.g., router to modem).

Cross-Layer Interaction:

The HTTP request is encapsulated into TCP segments, which are split into IP packets. These packets are further framed at the Link layer for transmission.
