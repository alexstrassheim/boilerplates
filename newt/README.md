
## Pangolin & NEWT

This project uses **NEWT** as a sub-component for **Pangolin**.  
You can find more information about Pangolin here:  
https://docs.pangolin.net/

> **Note:** Pangolin is running on an external server.  
> This repository does **not** describe how to install or operate Pangolin.  
> It only documents the **process of upgrading Pangolin**.

### Upgrading Pangolin

The official documentation for the update process can be found here:  
https://docs.pangolin.net/self-host/how-to-update

Always follow the instructions as provided in the official documentation.  
This README only serves as internal documentation for additional notes, steps, and guidelines.

### Upgrade from official documentation

1. `$ docker compose down`
1. Upgrade verison in `docker-compose.yml`
1. Optional upgrade version `config/traefik/traefik_config.yml`
1. `$ docker compose pull`
1. `$ docker compose up -d`
1. `$ docker compose logs -f`

