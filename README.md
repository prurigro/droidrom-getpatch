# droidrom-getpatch
========

## About: Once configured, this script will automatically download and patch the latest (or specified) OmniROM or CyanogenMod ROM for your device

## Requirements: To use this script, you'll need git, wget, md5sum, grep, sed, bash and a basic set of coreutils for things like echo

## Credits: Written by prurigro (https://github.com/prurigro | https://aur.archlinux.org/packages/?SeB=m&K=prurigro)

## License: Distributed under the GPLv3; copies can be obtained on gnu.org @ http://www.gnu.org/copyleft/gpl.html

## Usage:
* Open the script in a text editor
* Find where 'ROM_TYPE' is defined and set it to "omni" to download OmniROM or "cm" to download CyanogenMod
* Then find where 'DEVICE_NAME' is defined and set it to your phone's device string (the default "t0lte" is the Galaxy Note 2)
** You can find the list of supported models for the respective ROM @ http://dl.omnirom.org & http://download.cyanogenmod.org/
* Now find where 'AP_PATCHES' is defined and list the auto-patcher patches you want applied, each separated by a comma
** Available patches: pdroid,openpdroid,voice,v6supercharger,voice,insecure,secure,external_internal,tabletUI,3gdongle,pd2.0
* Optional: If you don't want the auto-patcher folder to be maintained in $HOME, change the 'AP_PARENTDIR' definition to your preferred location
** If the repo does not exist in the folder set here when the script is run, a new copy will be cloned
* Optional: If you want to use a different source for the auto-patcher repository, change the 'AP_GITREPO' definition to the alternative location
* Run droidrom-getpatch to get and patch the latest ROM, or specify a date or built type for a specific build
** Build types are special releases, such as "RC2", which CyanogenMod has used for a ROM's second release candidate
** The date should be written like: YYYYMMDD (eg: 20140127)
