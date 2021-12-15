# Janus Webrtc Gateway Test Server Docker With HTTPS Configured

- To Simply *Test the Screen Sharing Plugin* was the solo intent of creating this fork
- Since the plugin require HTTPS config and was thus not enabled on the official demo page
- And I did not found any repo that provided a one-click solution

## Usage

```sh
git clone https://github.com/cteamEpic/janus-webrtc-gateway-docker
cd janus-webrtc-gateway-docker

docker-compose up
  # (It may take awhile to build)

# Then simply visit the Demo Page
# (ignore the browser https unsafe warning since our https server used a self-signed x509 cert)
# Good to go
https://127.0.0.1:8443/screensharingtest.html
```

## Original Repos

- [Janus Gateway Repo](https://github.com/meetecho/janus-gateway)
- The `Dockerfile` is modified based on the [atyenoria Repo](https://github.com/atyenoria/janus-webrtc-gateway-docker)