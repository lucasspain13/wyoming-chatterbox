# Wyoming Chatterbox

## Local Install

Clone the repository and set up Python virtual environment:

```sh
git clone https://github.com/rhasspy/wyoming-piper.git
cd wyoming-piper
script/setup
```

Install Piper

```sh
curl -L -s "https://github.com/rhasspy/piper/releases/download/v1.2.0/piper_amd64.tar.gz" | tar -zxvf - -C /usr/share
```

Run a server that anyone can connect to:

```sh
script/run --piper '/usr/share/piper/piper' --voice en_US-lessac-medium --uri 'tcp://0.0.0.0:10200' --data-dir /data --download-dir /data
```
