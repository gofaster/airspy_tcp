# airspy_tcp
## a rtl-tcp compatible, IQ server for airspy SDR

airspy_tcp is a direct port of [rtl_tcp](https://github.com/osmocom/rtl-sdr) for the [airspy](https://airspy.com/).

As the rtl_tcp protocol is only 8 bits IQ, man will loose the major advantage of an airspy : its 12bits DAC, but :

1. It will work with any rtl_tcp capable frontend (Well I hope, see below)
2. As it's opensource, you could compile it on any Linux (and perhaps other UNIXes) server

Notes :
 - I try it with gqrx and sdrangelove frontend only. Other tests are welcome.
   Works as a gr-osmosdr source.
 - The rtl_tcp frontend client must set one the frequencies that the Airspy supports. Other sample frequencies are not supported.
 - Works with Airspy R0/R2 and Mini.
