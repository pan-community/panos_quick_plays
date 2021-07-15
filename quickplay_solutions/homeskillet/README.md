# HomeSkillet Quickplay Solution

HomeSkillet is a home-based deployment configuration as an Internet Gateway
using 2 zones, the untrust zone as a dhcp-client.

The security policy provides for outbound policies using IronSkillet
best practice security profiles and groups.

## Prerequisites 
The following should be completed before running the HomeSkillet Quickplay Solution:

    1. Deploy a PAN-OS 10.X NGFW
    2. License NGFW with the Threat, URL, and WildFire subscriptions
    3. Install PanHandler (Version 4.5+) or other skillet-supported applications, such as SLI
    4. Have DHCP-based public ethernet interface for L3 or L2/L3 mode
    5. Configure the NGFW for IronSkillet

> **NOTE**: You must have IronSkillet configured on your NGFW before loading the HomeSkillet solution 
> since many HomeSkillet configuration elements depend on IronSkillet elements.

## Submodules Utilized

This quickplay solution uses the [panos-config-elements](https://gitlab.com/panw-gse/tech-library/configure/panos-config-elements) 
repository as a submodule.

## Detailed Description

HomeSkillet currently supports L3 routing, hybrid L2/L3 routing, and virtual wire (vwire) options.

    * L3 Routing
        * One static Internal L3 interface and zone networking components
        * One DHCP Internet L3 interface and zone networking components
        * Virtual routing configurations
        * NAT rulebase configurations
        * DHCP local server
    * Hybrid L2 Switching with L3 routing
        * 2 zone configuration using an external Ethernet port and Internal VLAN logical interface
        * N number of interfaces are added to the Internal L2 switching zone based on user selection
        * NAT rulebase configurations
        * DHCP local server shared across the Internal Ethernet interfaces
    * Virtual Wire Routing
        * One Internal vwire interface and zone
        * One Internet vwire interface and zone
        * Virtual wire between the 2 interfaces

More details can be found at the [HomeSkillet docs page](https://homeskillet.readthedocs.io/).
