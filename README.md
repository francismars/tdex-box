# tdex-box
Docker Compose for running TDex Daemon with TLS along with the TDex Feeder. 

## Usage

1. Clone this repository.

```
$ git clone https://github.com/TDex-network/tdex-box/
```

2. Create [config.json](https://github.com/TDex-network/tdex-feeder#config-file) file.

3. Export ENV for the path of the config to be used.

```
$ export CONFIG_PATH=./config.json
```

4. Export ENV for the path of the SSL Certificate and Key to be used.

```
$ export SSL_CERT_PATH=./cert.pem
$ export SSL_KEY_PATH=./key.pem
```

### Run

```
$ docker-compose up -d
```

### Check the Logs

```
$ docker logs tdexd
$ docker logs feederd
```