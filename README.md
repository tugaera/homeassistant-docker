# homeassistant-docker

https://www.home-assistant.io/blog/2017/11/29/hassio-virtual-machine/
```
apt-get install -y apparmor-utils apt-transport-https avahi-daemon ca-certificates curl dbus jq network-manager socat software-properties-common

mkdir -p /home/pi/hassio
mkdir -p /mnt/volume/hassio
curl -sL "https://raw.githubusercontent.com/home-assistant/hassio-installer/master/hassio_install.sh" | bash -s -- -m raspberrypi4 -d "/home/pi/hassio"
```

https://www.zigbee2mqtt.io/information/docker.html
```
docker run \
   -it \
   -v $(pwd)/homeassistant:/app/data \
   --device=/dev/ttyACM0 \
   -e TZ=Europe/Amsterdam \
   -v /run/udev:/run/udev:ro \
   --privileged=true \
   koenkk/zigbee2mqtt
   
   ```
   
https://www.zigbee2mqtt.io/integration/home_assistant.html
