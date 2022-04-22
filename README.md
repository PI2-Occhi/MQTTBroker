# Eclipse MQTT Broker

Broker to enable MQTT protocol communication. Using the open-source [eclipse](https://mosquitto.org/) server.

## Setup Instructions
The setup can be done with or without docker. Using it is recommended to avoid environment-related errors. After launching the broker, it will be available on port 1883.

### Using [Docker](https://www.docker.com/) and [Docker-compose](https://docs.docker.com/compose/).

1. Clone the repository and enter its directory
2. Run `docker-compose up` to power on the message broker. The flag `-d` can be specified to omit logs and run the task in the background.

### Without Docker

1. Install mosquitto server: `sudo apt-get install mosquitto`
2. Launch the broker specifying the config file, `mosquitto -c config/mosquitto.conf` 