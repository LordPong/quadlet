# Pihole
This quadlet is designed to run a Pihole with Unbound recursive DNS inside a Pod named
`pod_pihole` on Podman, preferably under Fedora CoreOS

At the moment this files will only run in rootful mode.

## Installation
* Modify parameters to your needings (for example the `Environment=WEBPASSWORD=` variable for the pihole)
* Place the files `cnt_pihole.container` and `cnt_unbound.container` in the directory `/etc/containers/systemd/`
* Place the file `pod-pod_pihole.service` in `/etc/systemd/system/`
* Reload the systemd-daemon
* Enable the the Pihole pod
