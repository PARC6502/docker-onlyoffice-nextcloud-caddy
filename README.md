## Document Server and Nextcloud Docker installation with automatic HTTPS

Document Server and Nextcloud Docker installation will install the preconfigured version of [ONLYOFFICE Document Server][2] connected to Nextcloud to your server running them in Docker containers.

## Requirements

- The latest version of Docker (can be downloaded here: [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/))
- Docker compose (can be downloaded here: [https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/))

## Installation

1. Get the latest version of this repository running the command:

   ```
   git clone https://github.com/PARC6502/docker-onlyoffice-nextcloud-caddy.git
   cd docker-onlyoffice-nextcloud-caddy
   ```

2. Add domain and email to the Caddy section of the docker-compose.yml
3. Run Docker Compose:

   ```
   docker-compose up -d
   ```

   **Please note**: you might need to wait a couple of minutes when all the containers are up and running after the above command.

4. Now launch the browser and enter the webserver address. The Nextcloud wizard webpage will be opened. Enter all the necessary data to complete the wizard.

5. Go to the project folder and run the `set_configuration.sh` script:

   ```
   bash set_configuration.sh
   ```

Now you can enter Nextcloud and create a new document. It will be opened in ONLYOFFICE Document Server.
