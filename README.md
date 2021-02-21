# Three-Node Network communication via DTN on Google Cloud Platform and Windows Azure :rocket:
This project has been developed by Dr Lara Suzuki :woman_technologist: [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/larasuzuki.svg?style=social&label=Follow%20%40larasuzuki)](https://twitter.com/larasuzuki) and supervised by Vint Cerf :technologist: [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/vgcerf.svg?style=social&label=Follow%20%40vgcerf)](https://twitter.com/vgcerf), both at Google Inc.

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lasuzuki/StrapDown.js/graphs/commit-activity)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
![Profile views](https://gpvc.arturio.dev/lasuzuki)
[![GitHub contributors](https://img.shields.io/github/contributors/Naereen/StrapDown.js.svg)](https://GitHub.com/lasuzuki/StrapDown.js/graphs/contributors/)
[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![saythanks](https://img.shields.io/badge/say-thanks-ff69b4.svg)](https://saythanks.io/to/lasuzuki)

[![ForTheBadge built-with-science](http://ForTheBadge.com/images/badges/built-with-science.svg)](https://GitHub.com/lasuzuki/)

# Introduction
This is the third 5th tutorial on a series of DTN on Google Cloud tutorials. In the [first tutorial](https://github.com/lasuzuki/dtn-gcp), we introduced the ION software and its main functionalities, in addition to an intro to Google Cloud VMs.

In this tutorial we will introduce you to Windows Azure, and how to configure a 3-node network using ION. The figure below shows the network we will be building. Note that this example network uses two different convergence layers: TCP and LTP. This can illustrates the case of a terrestrial connection with two interplanetary internet nodes.

<img src="https://github.com/lasuzuki/dtn-gcp-ltp-tcp/blob/main/blob/network_arch.png" width=600 align=center>

# Three-Node Network

In this section, we assume that `host 1` has an IP address of 10.0.0.1, `host 2` has an IP address of `10.0.0.2`, and `host 3` has an IP address of 10.0.0.3. Please modify this for your uses. Please note that in this tutorial we are not covering routing, therefore, `host2` cannot communicate with `host3`. The routing tutorial can be found here.

This network is created by running the following command on `host 1`
````
ionstart -I host1.rc
````
This command is run on `host 2`:
````
ionstart -I host2.rc
````
Finally, this command is run on `host 3`
````
ionstart -I host3.rc
````





