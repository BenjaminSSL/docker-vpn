# A VPN as a docker compose file

This VPN is made from three essential components:

-   **Wireguard** for the VPN protocol
-   **Unbound** for the DNS caching and resolving
-   **AdGuard** Home for the ad blocking (DNS Sinkhole)

## Installation

The VPN should be installed on a server, and not on a local machine. The server needs an outward facing IP address, and the following ports should be open:

-   51820/udp

The server should also have Docker and Docker Compose installed. The installation of these is outside the scope of this README.

The installation of the VPN is done by cloning this repository and
running the `docker-compose` command.

```bash
git clone https://github.com/BenjaminSSL/docker-vpn.git
```

## Configuration

The VPN is configured by the environment variables in the `docker-compose.yml` file.

## Usage

The VPN is started by running the `docker-compose up -d` command. This will start the containers in the background (detached mode).

It can be stopped by running the `docker-compose down` command.

Please note that you need to run the `docker-compose` commands in the same directory as the `docker-compose.yml` file.

## Setup

TODO: Connecting with wireguard and adguard setup
