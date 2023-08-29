# Alfa-Driver-Install
For the Alfa adapter below, for Kali Linux.
https://www.amazon.com/Alfa-Long-Range-Dual-Band-Wireless-External/dp/B00VEEBOPG/ref=asc_df_B00VEEBOPG/?tag=hyprod-20&linkCode=df0&hvadid=309777534894&hvpos=&hvnetw=g&hvrand=291191125326881879&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9004087&hvtargid=pla-406165012713&psc=1&tag=&ref=&adgrpid=58425267301&hvpone=&hvptwo=&hvadid=309777534894&hvpos=&hvnetw=g&hvrand=291191125326881879&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9004087&hvtargid=pla-406165012713

## Step One:
Open Up the Terminal as Root (Red Terminal)

## Step Two:
Prepare for install. Run all three commands, one at a time in the terminal.
```
apt-get update
```
```
apt-get upgrade -y
```
```
apt-get dist-upgrade -y
```

## Step Three:
Install dkms. Run all two commands, one at a time in the terminal.
```
apt-get install dkms
```
```
apt-get install realtek-rtl88xxau-dkms
```

## Step Four:
Download the GitHub Driver Repository. Run the command in the terminal.
```
git clone https://github.com/aircrack-ng/rtl8812au.git
```

## Step Five:
Reboot. Run the command in the terminal.
```
reboot
```

## Step Six:
Open the root terminal (red terminal) once again.

## Step Seven:
Install Drivers. Run the three commands in the terminal, one at a time.
```
cd rtl8812au
```
```
make
```
```
make install
```

## Step Eight:
Reboot. Run the command in the terminal.
```
reboot
```

## Step Nine:
Plug in your Alfa Wifi Adapter, and open root terminal once again.

## Step Ten (Final Step)
Check. Run the following command in terminal. And you should see your adapter (wlan0)
```
ifconfig
```


Your welcome!! If this was helpful, please star this repo!!
