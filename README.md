# Asus TUF keyboard color changing utility on LINUX
Tested on FX505DT Keyboard LED
For supported laptops look at [here](https://github.com/hackbnw/faustus#systems)


# *EXPERIMENTAL*

How to use?
Install these beforehand.
1. make
2. dkms
3. zenity

Now run these command to get [Faustus driver](https://github.com/hackbnw/faustus)
```
git clone https://github.com/hackbnw/faustus.git
cd faustus
sudo make dkms
sudo make onboot
sudo sh -c "echo blacklist asus_wmi >> /etc/modprobe.d/blacklist.conf"
sudo sh -c "echo blacklist asus_nb_wmi >> /etc/modprobe/blacklist.conf"

```
REBOOT

----
Clone repo , and run keyled.sh , you can bind it to some keybinding if you want to.

What's working? Everything ( Haven't included fan suppport as of yet)
