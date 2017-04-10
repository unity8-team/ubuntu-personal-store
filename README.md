# Building

## Prerequisites

Ubuntu personal store is built as a snap package. That means that you only need snapcraft in order to build it.

     sudo apt install snapcraft

## Building

Once you have snapcraft installed in your system just go to the root of the project and run:

     snapcraft

A new ubuntu-personal-store_<version>_<arch>.snap will be created.

# Installing

Once you have a snap built locally, you can test it on your system by doing:

     snap install ubuntu-personal-store_<version>_<arch>.snap --devmode

The --dangerous flag is necessary for installing locally built snaps, which
have not been signed by the store.
The --devmode flag is necessary for authentication with gksu. We should be able to remove this option 
after we have a working PAM interface in snapd.

# Using

Just run the command:
     ubuntu-personal-store


