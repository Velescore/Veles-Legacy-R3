![Example-Logo](https://i.imgur.com/OP0aW7y.jpg?3)

Deprecation Warning
===================
This is the legacy version of Veles cryptocurrency software, third experimental public release. This version is no longer maintained and it will become incompatible after the block 50k by VCIP01 activation. 

It has been superseded by Veles Core R4 (v0.17): 
https://github.com/Velescore/Veles


Archive of Veles Core R3 (v0.16) integration/staging tree
=========================================================

https://veles.network

Linux Build Instructions and Notes
==================================

Dependencies
----------------------
1.  Update packages

        sudo apt-get update

2.  Install required packagages

        sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils libboost-all-dev

3.  Install Berkeley DB 4.8

        sudo apt-get install software-properties-common
        sudo add-apt-repository ppa:bitcoin/bitcoin
        sudo apt-get update
        sudo apt-get install libdb4.8-dev libdb4.8++-dev

4.  Install QT 5

        sudo apt-get install libminiupnpc-dev libzmq3-dev
        sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler libqrencode-dev

Build
----------------------
1.  Clone the source:

        git clone https://github.com/Velescore/Veles-Legacy-R3.git

2.  Build Veles Core:

    Configure and build the headless Veles Core binaries as well as the GUI (if Qt is found).

    You can disable the GUI build by passing `--without-gui` to configure.
        
        ./autogen.sh
        ./configure
        make

3.  It is recommended to build and run the unit tests:

        make check


Mac OS X Build Instructions and Notes
=====================================
See (doc/build-osx.md) for instructions on building on Mac OS X.



Windows (64/32 bit) Build Instructions and Notes
=====================================
See (doc/build-windows.md) for instructions on building on Windows 64/32 bit.
