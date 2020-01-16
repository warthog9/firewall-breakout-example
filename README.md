# firewall-breakout-example
This is an example / starting point set of configurations to help illustrate a firewall that's separated out. Not intended to be a running setup

# *** WARNING *** 
These files are provided as examples at best, and are not intended to be
actually working examples.  The IP addresses have been modified to have some
semblance of privacy.

A number of things have been removed from these configurations that are
actually being used cutting the resulting iptables commands down roughly half.

The blacklisted IPs are for example purposes only, and no commentary
is made about them beyond that they are present as examples. (to my 
knowledge, as of the writing of this, those IPs are currently not even
routable and unused. That can obviously change in the future)

There are a number of pieces that are not explained as to the reasoning why
ports are, or are not, opened.  I will not be going into any sufficient
detail as to why.  The only one that may be of any real mystery that's
interesting is having ports open on wlgst to fw, and the same items
being broadcast back into another network. This is to facilitate certain
protocols traversing network segments, like having your guests have the 
ability to cast to a chromecast device from the wireless guest network
( mDNSbi/ACCEPT ) or control other certain things that are not on the
"main" network.
