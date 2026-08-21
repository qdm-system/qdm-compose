# QDM Compose

## Installation

1. Clone the repo & install Docker

    ```bash
    git clone https://github.com/qdm-system/qdm-compose.git
    cd qdm-compose
    sudo ./install-docker.sh
    ```

2. Check then config

    Admin can modify systemm setting at [./docker/config.yaml](./docker/config.yaml), e.g. the default login credential:

    ```yaml
    username: "admin"
    password: "0000"
    ```

    For other setting, please make sure the modification is match the setting at [docker-compose.yaml](docker-compose.yaml).

3. Up the compose

    ```bash
    docker compose up
    ```

    The default db will be stored at `/var/lib/qdm/` which is mounted in the compose file.

4. Down the compose

    ```bash
    docker compose down
    ```
