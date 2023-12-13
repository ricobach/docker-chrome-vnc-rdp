# Google Chrome via VNC or RDP

Google Chrome via VNC or RDP container based on Ubuntu 16.04

[![Docker Build Status](https://img.shields.io/docker/build/ricobach/chrome-vnc-rdp.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/automated/ricobach/chrome-vnc-rdp.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/pulls/ricobach/chrome-vnc-rdp.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/stars/ricobach/chrome-vnc-rdp.svg?style=flat-square)]()

## Usage

### Build container
```
docker build -t sfoxdev/chrome-vnc-rdp .
```

### Run container without password

```
docker run -d -p 5900:5900 -p 3389:3389 --name chrome sfoxdev/chrome-vnc-rdp
```
### Run container with password

```
docker run -d -e PASSWORD=mypassword -p 5900:5900 -p 3389:3389 --name chrome sfoxdev/chrome-vnc-rdp
```
