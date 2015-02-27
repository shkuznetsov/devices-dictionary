# Devices dictionary
A humble attempt to collect widely dispersed data on how Cordova/Phonegap ``device.model`` value converts into a human-readable string.

### Why?
Cordova/Phonegap [device plugin](https://github.com/apache/cordova-plugin-device) reports device's model in a manufacturer-defined format, which is not particularly human-readable (e.g. "iPad4,5" instead of "Apple iPad mini 2" or "GT-I9300" instead of "Samsung Galaxy S III"). In my project I desperately needed that sorted in order to provide meaningful stats to an end-user, so I went on the internet looking for a comprehensive lookup database, but only found a few platform-specific ones, maintained by different people and provided in different formats. Since I needed them all in one place and format I thought I'd collate their data and opensource the result so that as many people as possible will be able to benefit from it. Please refer to "Tanks" section for a list of data sources I used.

### Data
Folder ``/files`` contains compiled data files in various formats:
* CSV
* JSON
* PHP
* SQL

``full.*`` files contain following fields:
* Model code as reported by ``device.model`` (e.g. "iPad4,5")
* Manufacturer (e.g. "Apple")
* Human-readable model name (e.g. "iPad mini 2")
* Platform (e.g. "iOS")
* Comment (e.g. "Retina/2nd Gen, Wi-Fi/Cellular")

``short.*`` files contain only model codes (e.g. "iPad4,5") and human-readable device names (e.g. "Apple iPad mini 2") -- and that is probably what you really need.

### Disclaimer
I have just started collecting the data, so it may be very uncomprehensive. Please report all the issues or send me a pull request.

### Todo
* Add Windows Phones and BlackBerries
* [Better] automate formats conversion
* Add [even] more formats
* Add basic SDKs

### Thanks (original data sources)
* [meetup/android-device-names](https://github.com/meetup/android-device-names) project on GitHub
* [Apple Model Number registry](http://www.everyi.com/by-identifier/ipod-iphone-ipad-specs-by-model-number-family-number.html) at Everyi.com

## License
MIT
