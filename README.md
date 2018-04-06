Install RedHat OpenShift Origin in your development box.

## Installation

1. Define mandatory variables for the installation process

```
# Domain name to access the cluster
$ export DOMAIN=<public ip addres>.nip.io

# User created after installation
$ export USERNAME=<current user name>

# Password for the user
$ export PASSWORD=password
```

2. Define optional variables for the installation process

```
# Instead of using loopback, setup DeviceMapper on this disk.
# !! All data on the disk will be wiped out !!
$ export DISK="/dev/sda"
```

3. Run the automagic installation script as root:

```
curl https://github.com/rdclicks/openshift/master/install-origin.sh | /bin/bash
```

## Development

For development it's possible to switch the script repo

```
# Change location of source repository
$ export SCRIPT_REPO="https://github.com/rdclicks/openshift/master"
$ curl $SCRIPT_REPO/install-origin.sh | /bin/bash
```

