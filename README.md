This is my linuxcnc config

both configs are working 
the test-pnc is more reliable > i dont have a closed loop configuration, but the config has a PID

my setup is a XXYZ Router
1000x600x120mm

i use a 2.2kw Chinaspindle with a the ER20 Collet (fits Milling bits up to 14mm)
watercooled > quiet setup
i use car coolant with distilled water 1:5 (the water does not become moldy and does not begin to stink)
Driver is a Huanyang > made a Mod to the Fan
AFB0512LB 5015 50x50x15mm with the VHM-802 and a DC-DC Converter Modul Buck Step-Down 24v to 12v

Raspberry PI 3 SPI MESA 7i90HD
for the OS i use the Realtimepi distro https://github.com/guysoft/RealtimePi
Mods   /etc/rc.local
add 
echo -n 1200000 > /sys/devices/system/cpu/cpufreq/policy0/scaling_min_freq
echo -n performance > /sys/devices/system/cpu/cpufreq/policy0/scaling_governor

LinuxCNC i installed a precompiled version form here
https://gitlab.com/orangecnc/installer/-/tree/master/linuxcnc
the armhf 2.8 (32 Bit OS)

Max feedrate 12000MM/Min
