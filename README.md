# Automation kit usb relay

This repo contains the files needed to source components and assemble the USB relay device that is to be used as part of the autmoation kit suite. 

![block-diagram](documentation/images/block-diagram.pdf)

The device is built around an off the shelf USB relay, with an enclosure built around it for both safety and ease of use.

To control the USB relay, the following tool can be used: https://github.com/darrylb123/usbrelay
The quickest way to use it is to install the package:

```
sudo apt-get install usbrelay
```

And then toggle with:
```
sudo usbrelay PSUIS_1=0
```

## Capabilities

- Toggle mains power via USB

## Interface

### Hardware

- C14 power input to connect to mains
- C13 output to connect to plug adapter for country/region its being used in
- USB A to connect to the host that will control the relay

### Software

- Open source control library: https://github.com/darrylb123/usbrelay
- Enables command line control, or python library