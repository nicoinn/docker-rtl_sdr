# Docker-rtl_sdr

A Docker container for building and executing rtl_sdr tools: http://sdr.osmocom.org/trac/wiki/rtl-sdr

The image is sized-optimized by using a multi-stage build and implements a minimalistic subset of the RTL-SDR toolbox (basically, only rtl_sdr )

# Usage

Obtain the image from the docker hub:

```docker pull nicoinn/rtl-sdr```


Run an rtl-sdr tool from the container (this will work only on a Linux host):

```docker run --privileged -v /dev/bus/usb:/dev/bus/usb nicoinn/rtl-sdr```
