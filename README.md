# Install & Configure Raspberry pi via Ansible scripts

## Prerequisites

1. Download RaspiOS from https://downloads.raspberrypi.org/raspios_lite_armhf/images/raspios_lite_armhf-2023-05-03/ and save to SD card.

1. Copy files from project `SD`` folder to `boot` partition on SD card.

1. Install Ansible requirements:
    ```sh
    ansible-galaxy install -r requirements.yaml
    ```

## Deploy
```sh
ansible-playbook -i inventory.yaml site-domoticz.yaml
```

**NOTE:** Tested with `Ansible v2.10.8`, `Python v3.10.12` and `RaspiOS lite 2023-05-03`.