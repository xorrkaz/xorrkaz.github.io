# Getting To Know YDK

New to the concepts behind model-based management?  Maybe you've heard of YANG, but you're not sure
how to navigate YANG modules to find what you're looking for.  Or maybe you've found the YANG path
that will do what you want, but you're not sure how to use it to achieve your desired results.

The one thing you do know is that you need to automate stuff.   You need to scale the creation of
new services from the application down to the network.  You want to take the concepts you've been
used to when it comes to network configuration, and get them plugged in to an automation framework
that will give you quick and reliable control over your network operations.

Let's say you have a campus network composed of Catalyst 3850 switches, and you want to
programmatically create new VLANs on these switches using YANG-based NETCONF.  You want to create
a Python script that will push the VLAN changes to the required switches.

First, let's make sure YANG-based NETCONF is enabled on the device.  To do that, do the following:

```
Switch#config t
Switch(config)#netconf-yang
```
