cm-getpatch
========

About: This script will automatically download and patch the latest (or recent if specified) Cyanogenmod ROM for your device

Requirements: To use this script, you'll need git, wget, md5sum, grep, sed, bash and a basic set of coreutils for things like echo

Usage:
    1. Open the script in a text editor
    2. Set the $DEVICE_NAME variable to the name of your device (which can be found on get.cm)
    3. Customize the $AP_PATCHES variable with the patches you would like built for your ROMs, each separated by a comma
        * Available patches: pdroid,openpdroid,voice,v6supercharger,voice,insecure,secure,external_internal,tabletUI,3gdongle,pd2.0
    4. Set the $AP_PARENTDIR variable to the directory the script should expect to find the auto-patcher repo
        * If the repo does not exist when the script is run, a new copy will be cloned
    5. Most people shouldn't need to change the $AP_GITREPO variable, but it's available should someone have a need to do so
    6. Run the script to download and patch the latest ROM, or run the script with a specific date to download the ROM from that day
        * The date should be written like: YYYYMMDD (eg: 20130826)
