# Drone prototype requirements

Prototype is assumed to be a "CO2 sensor thing" which can be attached to some generic "platform".

## WoT interface

The [Wot Specification](https://www.w3.org/Submission/wot-model/#resources) defines endpoints for Model, Properties and Things.

```
/model --  A web Thing always has a set of metadata that defines various aspects about it such as its name, description, or configurations.
/things -- A web Thing can be a gateway to other devices that don’t have an internet connection. This resource contains all the web Things that are proxied by this web Thing. This is mainly used by clouds or gateways because they can proxy other devices.
/properties -- A property is a variable of a web Thing. Properties represent the internal state of a web Thing. Clients can subscribe to properties to receive a notification message when specific conditions are met; for example, the value of one or more properties changed.