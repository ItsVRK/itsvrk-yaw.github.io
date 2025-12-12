# Update or restore SD Card for Yaw 3

If you want to modify the chair to support [Wifi6E then skip to here](wifi6e.md)

Prior to doing this you should execute the following on the chair:

SSH into the device, substitute with the IP of your simulator on your network:

`ssh pi@192.168.0.120` The password is pi

Then execute the following command and store the output:
`sed -n 's/^License=//p' /usr/local/etc/virtualhere/config.ini`

The output is your VirtualHere license, save this! you will need this if your SD ever gets corrupted and you need to reflash the SD, without it you will probably need to re-purchase VirtualHere, as long as you have this you can relicense VH on the same physical Raspberry Pi.

## Updated RaspberyPi OS Stock Image

Flash the following image to SD card using <a target="_blank" href="https://etcher.balena.io/">Balena Etcher</a>

<a target="_blank" href="https://www.dropbox.com/scl/fi/z3sw98az1iv9dd7d81ekb/YawIII-RaspberryPIOS12-clean-opt.zip?rlkey=op915xaa90l3ocizqkcvj2ovu&st=o4hwm8b4&dl=0">YawIII-RaspberryPIOS12-clean-optimized</a>
