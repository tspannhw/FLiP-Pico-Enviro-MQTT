# FLiP-Pico-Enviro-MQTT

MQTT from Pimoroni Pico W Enviro Indoor

### Configuration

Set MQTT Broker Name to IP address of Pulsar.   It will auto add 1883 as port

### Configuration will determine topic name and it will be auto created

### Pulsar Consume Data CLI

````
bin/pulsar-client consume "persistent://public/default/enviro%2Fpulsar-conference-tracker" -s "indoorer" -n 0
````

### Example Data

````
----- got message -----
key:[null], properties:[], content:{"pressure": 1009.65, "temperature": 26.65, "timestamp": "2022-08-30 15:48:29", "color_temperature": 3052, "device": "pulsar-conference-tracker", "humidity": 41.23, "luminance": 12}

````

### Links

* https://github.com/pimoroni/enviro
* https://github.com/pimoroni/enviro/blob/main/documentation/getting-started.md
* https://shop.pimoroni.com/products/enviro-indoor?variant=40055644684371
* https://github.com/tspannhw/pulsar-adafruit-funhouse
