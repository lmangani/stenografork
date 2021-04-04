# Stenographer Docker

## Build
```
docker build -t qxip/stenographer .
```

## Usage
```
docker run \
  --net=host \
  --volume /var/steno:/var/lib/stenographer \
  --cap-add NET_ADMIN \
  --cap-add IPC_LOCK \
  qxip/stenographer \
  --interface enp0s3 \
  --indexbase /var/lib/stenograpapher/IDX \
  --packetsbase /var/lib/stenographer/PKT
 ```
