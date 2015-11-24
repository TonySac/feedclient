# ADS-B Exchange Setup Scripts :airplane:

Feeding ADSBexchange.com is quick and easy. There are various options depending on what kind of feeder/receiver you use,
and your desired level of customization. This script aids in setting up your current PiAware or Dump1090 based feeder to
feed ADS-B Exchange. Although not required it is recommended that FlightAware’s PiAware be used to feed data to
ADSB-Exchange in order to send the most accurate MLAT results to the co-op.

### Obtaining And Using The Scripts

Running the following commands will download the contents of this repository.

    sudo apt-get install git
    git clone https://github.com/jprochazka/adsb-exchange.git
    cd adsb-exchange
    chmod +x setup.sh
    sudo ./setup.sh
    
**After completing the setup do not delete this repository.**

The file adsbexchange-maint.sh script resides in this folder containing a clone of this repository. The path to execute this script after a reboot has been set to this location. Deleting this folder will result in the adsbexchange-maint.sh script not being executed thus not enabling your feeder to feed ADS-B Exchange.

**no_dialogs.sh**

The file "no_dialogs.sh" can used in place of "setup.sh" to set up your receiver.  
The only difference between the two files is "no_dialogs.sh" does not use Whiptail dialogs.

### Reporting Issues

Feel free to report any issues you encounter either in this repositories issue tracker or the ADS-B Exchange Setup Script
topic located in the ADS-B Exchange forums.

https://github.com/jprochazka/adsb-exchange_setup/issues  
http://www.adsbexchange.com/forums/topic/ads-b-exchange-setup-script/
