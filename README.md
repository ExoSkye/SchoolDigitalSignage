# SchoolDigitalSignage
Digital Signage Solution for my school

## Architechture

### Server
Windows Service acts as the server and uses TCP to send and recieve information

Written in C++ using ASIO

### Client
Raspberry Pis (armhf/arm64) running buildroot

Client written in C++ using SDL and libdrm

## User utilities

Controller GUI which connects to the server via TCP and allows rules to be set in an easy to use interface

## Capabilites

### Media types

- Images
- Text

### Visual effects

- Transitions
