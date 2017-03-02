# Thread Study Note #

## Introduction ##
![Overview of Thread Stack](Overview_of_Thread_Stack.jpg)

## Type and Role of Devices ##
* Full Thread Device (FTD)
  * Active Router
  * Router-Eligible End Device (REED)
  * Full End Device (FED)
* Minimal Thread Device (MTD)
  * Minimal End Device (MED)
  * Sleepy End Device (SED)
* Roles can be combined in any device
  * Leader
  * Border Router
  * Commissioner

FTDs can communicate with each other and with their attached MTD Children. MTDs can only communicate with the FTD Parent they are attached to.

### Router ###
Routers provide routing services to network devices. Routers also provide joining and security services for devices trying to join the Thread Network.

After forming a network, the forming node becomes the first Router in the Thread Network partition and selects a Router ID for itself.

Devices initially attach to the Thread Network as a REED, and may request to become Routers at any time after attaching.

### Leader ###
There is a device acting as the Leader. And there can be only **ONE** Leader at a time.

The Leader's main functions:
* Assign and manage Router IDs.
* Collate and distribute the Thread Network Data.

### Border Router ###
A Border Router is a device capable of forwarding between a Thread Network and a non-Thread Network. There may be one or more Border Routers in a Thread Network.

### Commissioner ###
There is an on-mesh commissioning device or an off-network commissioning device, a mobile phone or a server in the cloud, acting as the Commissioner. There can be only **ONE** active Commissioner at a time.

The Commissioner is the currently elected authentication server for new Thread devices and the authorizer for providing the network credentials they require to join the network, and typically provides the interface by which a human administrator manages joining a new device to the Thread Network.

## Forming a Network ##


## Joining a Network ##

### Commissioning ###

### Joining ###


> ## Reference ##
> 1. Thread v1.1.0 Specification
> 2. Thread Technical Overview (5 October 2015 Berlin)
