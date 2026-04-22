# foolstrap
Fool's trap is a lightweight Windows x64 program that sends back a fake banner as a reponse of a scan or request.

As a socket listening server Fool's trap wait for an incoming connection on a TCP port on your Windows machine then reads the request of a client and sends a fake answer back to this client.

This tool can be used for:
- Cyberdeception
- Testing connectivity

It was tested on Windows 11 Home/Pro against telnet, nc and nmap.

By default Fool's trap listens on port TCP 11111.

# Installation

## Step 1: Downloading

Installation is easy: just download the executable.

## Step 2: Allowing the program to be launched

Actually there is no threat but Windows Defender displays a warning message after downloading the executable. To avoid Windows Defender blue screen "Windows protected your PC" you have 2 options:

1. Right click on the file, check "Unblock" then click "Apply" button.

![Unblock](images/unblock.png)

or

2. You run the executable then on the popup just click "More info" then "Run anyways".

![Windows protected your PC](images/windows_protect_your_pc.png)


## Step 3: Allowing access to the network (Windows Firewall)

Because the software use network connections to be connected to it then Windows Firewall shows another popup the first time to allow or block the application to get network access.

Just click "Allow" button.

![Windows Firewall](images/windows_firewall_alert.png)


# Usage

Run the program.

``` PowerShell
C:\>foolstrap.exe
Server running. Waiting for connection...
```

# Commands

Supported commands are:

"/v" or "-v" to get sofware version.

```PowerShell
C:\>foolstrap.exe -v
Fool's Trap 1.0.0 by Glacius

C:\>
```


