# FM Stereo with RDS Transmitter and Receiver


## Overview and Hardware

GNU Radio flowgraphs for a broadcast FM multiplex transmitter and receiver. Supports stereo audio and Radio Data System (RDS).

This code is designed for the ADALM-PLUTO SDR. However, it can be easily adjusted to other SDRs by changing the SDR source and sink blocks.

The following firmware change needs to be made on the ADALM-PLUTO to operate in the broadcast FM band (88-108 MHz): https://www.rtl-sdr.com/adalm-pluto-sdr-hack-tune-70-mhz-to-6-ghz-and-gqrx-install/


## Software Dependencies for functionality without RDS

* **GNU Radio Companion (with supported OS of your choice)**: https://wiki.gnuradio.org/index.php/InstallingGR


## Software Dependencies for functionality with RDS

* **Ubuntu/Debian/Linux Mint/Raspberry Pi OS 64-bit (Ubuntu recommended!)**

* **GNU Radio Companion**: https://wiki.gnuradio.org/index.php/InstallingGR

* **GR-RDS and its dependencies**: https://github.com/bastibl/gr-rds


### Additional commands I needed to get GR-RDS dependencies

```
sudo apt-get install cmake libblkid-dev e2fslibs-dev libboost-all-dev libaudit-dev
sudo apt install make
sudo apt-get install git
sudo apt-get install doxygen
sudo apt install graphviz
sudo apt-get install xterm
```

## Files

* **Project_Report.pdf**: Information about FM stereo, RDS, and this implemenation
* **FM_RX_Test_noRDS.grc**: FM stereo receiver without RDS support
* **FM_TX_Test_noRDS.grc**: FM stereo transmitter without RDS support
* **FM_RX_Test_RDSver(x).grc**: FM stereo receiver with RDS support (different demodulation schemes - details on page 10 of "Project_Report.pdf")
* **FM_TX_Test_RDS.grc**: FM stereo transmitter with RDS support
* **Test_WAV.wav**: Sample stereo audio file for transmitter - "Give It Up (Start Again)" by Snowflake feat. Subliminal. The track is licensed by Creative Commons. Download it for free at https://bandcamp.musikpiraten-ev.de/track/give-it-up-start-again-feat-subliminal

## Folders
* **Flowgraph PDFs**: Contains PDFs of the above listed grc flowgraphs.

