# ☭psfs
A GPS filesystem with Soviet assistance

The proper name is ☭psfs, but github cut the little hammer and sickle out of the name.

This was made to work with the PA1616D GPS reciever.

It uses multiple types of positioning satellites, and will prefix location and other NMEA sentances with $GN instead of the $GP used for just American GPS data.  This is just a modification of the gpsfs program that comes with 9 Front so that it parses $GN sentances instead of $GP ones.
