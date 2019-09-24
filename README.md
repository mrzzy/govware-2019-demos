# Govware 2019 Exploit Demos

## Intro
This repository attempts to implement the following exploits for Govware 2019:
- Oracle WebLogic Server CVE-2019-2725
- Docker Runc CVE-2019-5736
with `docker` containers.

## Project Structure
The project is structured as follows:
- `weblogic/` - A Oracle WebLogic Server CVE-2019-2725
    - `containers/` - containers used in the exploit 
        - `attacker/` - attacker container
        - `victim/` - victim container
- `docker/` - Docker Runc CVE-2019-5736
