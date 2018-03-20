
https://www.perforce.com/perforce/r14.2/manuals/cmdref/index.html

https://www.perforce.com/perforce/doc.current/manuals/p4sag/Content/P4SAG/install.linux.packages.install.html

Configure the Helix Core package repository.
---
Create the file /etc/apt/sources.list.d/perforce.list with the following content:

deb http://package.perforce.com/apt/ubuntu xenial release

2. Import the Helix Core package signing key.

3.Install the appropriate Perforce service package.

The Perforce service is divided into multiple packages, so you can install just the components you need. The component package names are:

helix-p4d
helix-p4dctl
helix-proxy
helix-broker
helix-cli
The helix-p4d package installs the main component of a Perforce service, p4d, as well as the command line interface, the service controller, and a configuration script to set them up.

At minimum, you need to install the helix-p4d package. To install a different package, substitute its name for helix-p4d in the commands below.

Run one of the following:

For Ubuntu:

$ sudo apt-get update
$ sudo apt-get install helix-p4d

