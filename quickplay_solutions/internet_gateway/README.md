# Internet Gateway Quickplay Solution


## Prerequisites 
The following should be completed before running the Internet Gateway Quickplay Solution:

    1. Deploy a PAN-OS 10.X NGFW
    2. License NGFW with the Threat, URL, and WildFire subscriptions
    3. Install PanHandler (Version 4.5+) or other skillet-supported applications, such as SLI
    4. Configure the NGFW for IronSkillet

> **NOTE**: You must have IronSkillet configured on your NGFW before loading the Internet Gateway solution 
> since many Internet Gateway configuration elements depend on IronSkillet elements.

## Submodules Utilized

This quickplay solution uses the [panos-config-elements](https://gitlab.com/panw-gse/tech-library/configure/panos-config-elements) 
repository as a submodule.

## Detailed Description

The Internet Gateway panos skillet configures the following elements: 
