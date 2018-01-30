# ResinOS and Docker-compose

Use a [resinOS device](https://resinos.io/) as a remote host to [docker-compose](https://docs.docker.com/compose/overview/).

## Usage

### Setup your resinOS device.
Head over to the [getting started page of resinOS](https://resinos.io/docs/odroid-ux3/gettingstarted/)
1. Download recent resinOS device image, example: [Odroid XU4 2.9.7].(https://github.com/resin-os/resin-odroid/releases)
2. **[Optional]** [Configure](https://resinos.io/docs/odroid-ux3/gettingstarted/#configure-the-image) the image host name.
3. Power up the device and make sure its connected to the network.

### Install Docker and Docker-compose
Install docker + docker compose on your laptop, following this guide: https://docs.docker.com/compose/install/

### Deploy your services:
From the project directory run the following.
```
DOCKER_API_VERSION=1.22 DOCKER_HOST=tcp://192.168.0.42:2375 docker-compose up
```
