# Resting-Catt
A REST API wrapping skorokithakis/catt intended for Home Automation usage. Derivation of https://github.com/homeassistant-addons-eliseo/resting-catt

## BUILD

```
docker build . -t mirecekd/resting-catt
```

### RUN

```
docker run --name=resting-cat -p 9898:9898 --restart always mirecekd/resting-catt
```


### USAge

```
curl -X POST http://docker.server.local.lan:9898/cast_site \
     -H 'Content-Type: application/json' \
     -d '{"device":"address.of.chromecast.local.lan",\
          "url":"http://site.to.cast.to.chromecast"}'
```
