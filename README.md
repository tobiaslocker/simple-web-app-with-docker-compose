## Usage
### Adding certificate and key 
Put your server's certificate and key into a directory `certs`
```console
$ mkdir certs
$ cp /path/to/mydomain.com.crt ./certs
$ cp /path/to/mydomain.com.key ./certs
```
### Configure
Create `.env` file with your images/host
### .env
```
BACKEND_IMAGE=tobiaslocker/simple-dockerized-flask-backend:v0.1
BACKEND_VIRTUAL_HOST=backend.mydomain.com
BACKEND_VIRTUAL_PORT=8080
FRONTEND_IMAGE=tobiaslocker/simple-dockerized-react-frontend:v0.1
FRONTEND_VIRTUAL_HOST=mydomain.com
```
> :warning: **You need to set up backend.mydomain.com to point to the same IP as mydomain.com**
