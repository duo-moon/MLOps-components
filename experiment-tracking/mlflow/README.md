# mlflow

## Installation

#### Prerequisites
* Docker and Docker Compose

**1. Create `.env` file**

Create a `.env` file in the mlflow root directory (example file `./mlflow/.env.example`). Open file in a text editor and add the necessary environment variables. 

**2. Create `htpasswd` file**

Create a `htpasswd` file in the `./mlflow/var/nginx` for nginx server. This file will contain username and password in an encrypted format.
```bash
htpasswd -c ./var/nginx/.htpasswd username
```
**3. Run Docker Compose**
```bash
docker-compose up
```
