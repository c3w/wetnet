###
## wetnet v.1
## c3w@juicypop.net

## VIDEO @ http://www.youtube.com/watch?v=_Bw3m5Xogkw&feature=youtube_gdata_player

WetNET is a supernet-aware IPv4 provisioner, written in Python, with a MySQL DB

IP Routing protocols aggregate subnets into supernets, and so, WetNET is designed to
provision subnets and hosts within ranges, allocated to Layer 3 devices.

Usage: wetnet [create|query] [supernet|set|subnet|host] x.x.x.x/x [device] device-id

Step one(1) is to create the supernet that your organization owns
Step two(2) creates 'sets' to be dedicated to subnetting a particular size subnet, e.g. /27s
Step three(3) outputs a subnet of allowed size, and tags it in the database
Step four(4) creates a host record in the database, within one of the allocated subnets

--c3w 2012092801
