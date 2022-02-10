# ☭psfs
A GPS filesystem with Soviet assistance

The proper name is ☭psfs, but github cut the little hammer and sickle out of the name.

This was made to work with the PA1616D GPS reciever, which is what I got on the Adafruit Ultimate GPS v3, even though they said it was supposed to be the PA1616S.

The PA1616D uses multiple types of positioning satellites, and will prefix location and other NMEA sentances with $GN instead of the $GP used for just American GPS data.  This is just a modification of the gpsfs program that comes with 9 Front so that it parses $GN sentances instead of $GP ones.

On Plan9 or 9Front;
Go into the ☭psfs directory
run 'mk install'

It works just like the version from 9Front, so check their man page for detials.

On my Raspberry Pi, to run it; 
aux/☭psfs -d /dev/eia0 -b 9600

for more info
https://youtu.be/Ij-J1xbVzfU
