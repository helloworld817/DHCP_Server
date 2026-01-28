DHCP Server in a Small LAN with WLC and Lightweight AP
Overview

This lab simulates a small enterprise LAN where both wired and wireless devices receive IP addresses from a centralized DHCP server.

The wireless network is managed using a Wireless LAN Controller (WLC) and a Lightweight Access Point (LAP).
The WLC does not provide DHCP itself — instead, it forwards DHCP requests to the server, ensuring centralized IP management.
-------------------------------------------------------------
Network Components

DHCP Server
  Provides IP addresses, subnet mask, default gateway, and DNS

Switch
  Connects wired devices, WLC, AP, and server

Wireless LAN Controller (WLC)
  Manages wireless network and SSIDs
  Forwards DHCP requests to the DHCP server

Lightweight Access Point (LAP)
  Joins the WLC and provides wireless coverage

Wireless Clients (Tablet/Laptop)
  Receive IP addresses via DHCP through WLC


IP Addressing Design
Device	IP Assignment
DHCP Server	Static IP
WLC (Management Interface)	Static IP
LAP	DHCP
Wired Clients	DHCP
Wireless Clients	DHCP

All clients (wired and wireless) are assigned IPs from the same DHCP server, ensuring consistent network configuration.
