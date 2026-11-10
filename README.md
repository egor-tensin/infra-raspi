infra-raspi
===========

Trying to make setup fully automated on my Raspberry Pi's.

Prerequisites
-------------

* Image the SD card with the RPI Imager (preferrably with the Lite OS version).
* `ssh-copy-id` your key to the target machines for `make init`.
* Ansible installed on the controller.

```
make init LIMIT=host
```

^^^ This step should be run on the local network, so that the hosts are
discoverable via .local hostnames.

Usage
-----

This should run the main playbook, setting up everything:

    make config

After everything is set up, maintenance can be done via the GitHub workflow.
