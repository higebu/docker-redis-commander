# Redis Commander Docker image

Docker image for [Redis Commander](https://github.com/joeferner/redis-commander)

[![Redis Commander Version](https://img.shields.io/badge/redis--commander-0.3.2-green.svg)](https://www.npmjs.com/package/redis-commander)

## Usage

* Show help

```
docker run -it --rm higebu/redis-commander --help
Options:
  --redis-port                    The port to find redis on.              [string]
  --redis-host                    The host to find redis on.              [string]
  --redis-socket                  The unix-socket to find redis on.       [string]
  --redis-password                The redis password.                     [string]
  --redis-db                      The redis database.                     [string]
  --http-auth-username, --http-u  The http authorisation username.        [string]
  --http-auth-password, --http-p  The http authorisation password.        [string]
  --address, -a                   The address to run the server on.       [string]  [default: "0.0.0.0"]
  --port, -p                      The port to run the server on.          [string]  [default: 8081]
  --nosave, --ns                  Do not save new connections to config.  [boolean]
```

* Run

```
docker run -d --name redis-commander -p 8081:8081 higebu/redis-commander --redis-host 192.168.100.5
```
