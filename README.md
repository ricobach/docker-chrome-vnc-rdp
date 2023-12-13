# Google Chrome via VNC or RDP

Google Chrome via VNC or RDP container based on Ubuntu 16.04 

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
