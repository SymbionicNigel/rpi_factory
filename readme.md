# Raspberry Pi Image Factory

In an effort to make use of my small [SBC collection](https://en.wikipedia.org/wiki/Single-board_computer), I will be assembling a toolchain and set of configurations to make the  process of deploying OS images as simple and reproducible as I can. I will attempt this by shoving as much of the process into [IAC](https://en.wikipedia.org/wiki/Infrastructure_as_code) and configuration files, with scripts to handle any manual actions.

## Initial plans

My first development initiative is to produce a POC which makes use of [pi-gen](https://github.com/RPi-Distro/pi-gen) to configure and automate the building of a [docker based OctoPrint](https://hub.docker.com/r/octoprint/octoprint) server image, preconfigured to run with as little interaction as possible after inserting the SD Card.

## Future Goals

- add more configurations to create other pre-canned images for raspberry Pis
- run this as part of a CI build pipeline sending artifacts off to a PXE boot server
