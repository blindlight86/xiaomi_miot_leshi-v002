# Xiaomi MIOT Leshi-v002
A simple example of a Home Assistant extension for Xiaomi 3rd party switch (leshi.switch.v002).
This only switches on/off the device.

# Install
You can install it manually by copying the custom_component folder to your Home Assistant configuration folder and restarting your Home Assistant.

# Setup
```
# configuration.yaml

switch:
  - platform: xiaomi_miot_leshi-v002
    name: Mi WiFi Switch X
    host: 192.168.1.152
    token: b110204d86732b019d3d6axxxxb9ad3a
```
Configuration variables (switch platform):

host (Required): The IP of your miio device.

token (Required): The API token of your miio device.

# Modification
Here is a guide how to control almost any Xiaomi MIOT device: https://github.com/rytilahti/python-miio/issues/901
You can fork this switch example and change "siid" / "piid" values according to your device's settings.
