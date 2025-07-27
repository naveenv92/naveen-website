+++
title = 'can-go'
date = 2024-04-26T19:19:40-07:00
draft = false
+++

![](/img/can_bus.jpg)
_Photo by Kumpan Electric on Unsplash_



Communication between the electronic control units (ECUs) in automobiles are sent using the Controller Area Network (CAN) protocol. These communications are represented as binary data packed into messages, which comprise of a set of signals from sensors all over the vehicle. In order to decode these binary payloads into human-readable data, we can use a DBC file that describes all the possible messages and signals. An example of a DBC and it's interpretation can be found at [this website](http://socialledge.com/sjsu/index.php/DBC_Format).

`can-go` is a package written in Go that is adapted from forked from a package from [Swedish automotive company Einride](https://github.com/einride/can-go) for decoding arbitrarily long CAN messages (the original CAN standard being limited to 8 byte payloads). It currently runs in production, processing terabytes of telematics data from the Rivian fleet daily.

__Link to github repo:__ https://github.com/jshiv/can-go
