# homeassistant-docker

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
