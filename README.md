---
page_type: sample
languages:
  - javascript
  - nodejs
products:
  - azure
  - azure-iot-hub
description: Sample of a simulator for Raspberry Pi.
---

# Raspberry Pi Web Client Simulator

[![Gitter](https://img.shields.io/badge/chat-on%20gitter-blue.svg)](https://gitter.im/Microsoft/raspberry-pi-web-simulator)

Click to visit **[Demo page](https://azure-samples.github.io/raspberry-pi-web-simulator/build/index.html)** This is the preview version and we'd like to have your feedback. You can submitt issues or chat with the product team in the gitter.

## How to register an IoT hub (we used 'horace.isa@gapp.nthu.edu.tw', PWD: 'h531????C')

Click [this page](https://docs.microsoft.com/azure/iot-hub/iot-hub-raspberry-pi-web-simulator-get-started) and follow it to create your own IoT hub

## Usage

- Replace the connection string with your Azure IoT hub device connection string, and click `run` button or type `npm start` in the console to run a client application to

    - send message to IoT hub
    - receive C2D message from IoT hub
    - receive device method from IoT hub

- While the sample code running, you can see

    - the LED is blinking in the left part
    - some message is printed in the console
    
- To expand the code editor, you can fold the console

- Write your own piece of code in the code editor and run

## Contribution Guide

**Notice!** Only `source` branch is for source code. `master` and `static-int` branch are generated by build service. So never manually update these branches.

### For common scenario

- Create a new branch based on `source` branch.
- Create a Pull Request.
- Merge with `source` branch with at least one approval. **Do not merge with git tags**
- Wait for 5 minutes and check your change on [test site](http://raspberry-pi-simulator.azurewebsites.net)

### For production deployment scenario

- Before doing following steps, make sure all changes are tested on test site.
- Create a tag with `git tag` command. Better name the tag as version number.
- Use `git push --tags` command to push tag on `source` branch.
- Wait for 5 minutes and check your change on [prod site](https://azure-samples.github.io/raspberry-pi-web-simulator/)
