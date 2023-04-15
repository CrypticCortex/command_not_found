Closing the lid turns on the aeroplane mode ? Irritating ?
Try [this](https://askubuntu.com/questions/1156932/ubuntu-18-04-goes-to-aeroplane-mode-when-i-close-the-lid).

Blutoothctl says ```No default controller available``` ?
Try the following :
```
sudo rmmod btusb
sudo rmmod btintel
sudo modprobe btintel
sudo modprobe btusb
```