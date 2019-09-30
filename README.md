# Govware 2019 Exploit Demos

## Intro
This repository attempts to implement the following exploits for Govware 2019:
- Oracle WebLogic Server CVE-2019-2725
- Docker Runc CVE-2019-5736
with `docker` containers.

## Setup
Prequisites for all exploits:
- Install `docker` and `docker-compose`

Instructions for Running demos:
1. Change directory to exploit (see Project Structure)
```sh
cd <exploit dir>
```
2. Download docker images 
```sh
docker-compose pull
```
3. Bring up the stack
```
docker-compose up
```
4. On another terminal, access the attacker machine using:
```
docker-compose exec attacker
```
5. Exploit

## Project Structure
The project is structured as follows:
- `weblogic/` - A Oracle WebLogic Server CVE-2019-2725
    - `containers/` - containers used in the exploit 
        - `attacker/` - attacker container
        - `victim/` - victim container
- `docker/` - Docker Runc CVE-2019-5736
    - `containers/` - containers used in the exploit 
        - `attacker/` - attacker container
        - `victim/` - victim container
