# Upgrade Yaw 3 to Wifi 6E

Prior to doing this you should execute the following on the chair:

SSH into the device, substitute with the IP of your simulator on your network:

`ssh pi@192.168.0.120` The password is pi

Then execute the following command and store the output:
`sed -n 's/^License=//p' /usr/local/etc/virtualhere/config.ini`

The output is your VirtualHere license, save this! you will need this if your SD ever gets corrupted and you need to reflash the SD, without it you will probably need to re-purchase VirtualHere, as long as you have this you can relicense VH on the same physical Raspberry Pi.

## Whats required

- [RPI PCIE Adapter board (MPW7N)](https://s.click.aliexpress.com/e/_oBgVflp)
- [AX210NGW Nic (AX210 10dbi Kit)](https://s.click.aliexpress.com/e/_oBzd06B)
- [Longer PCIE ribbon](https://amzn.to/4oOFzo0)
- [3D Printed mounting adapter, STL here](../../assets/3dmodels/yaw3-hat_mount.stl)

Flash the following image to SD card using <a target="_blank" href="https://etcher.balena.io/">Balena Etcher</a>

<a target="_blank" href="https://www.dropbox.com/scl/fi/e9qmyjaa4kf5834dsfl0g/YawIII-RaspberryPIOS12-wifi6E-opt.zip?rlkey=uhi4oinz3wbrz24ghkpc9n4go&st=gc2d5hpm&dl=0">YawIII-RaspberryPIOS12-wifi6E-opt.zip</a>

## How to install it

<video width="1280" height="720" controls>
  <source src="/assets/video/yaw3wifi6e.mp4" type="video/mp4">
Your browser does not support the video tag.
</video> 