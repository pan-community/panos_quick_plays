# eSports Quickplay Solution

The eSports Skillet is designed to create the baseline configurations necessary to support eSports.

## Prerequisites 
The following should be completed before running the eSports Quickplay Solution:

    1. Deploy a PAN-OS 10.X NGFW
    2. License NGFW with the Threat, URL, and WildFire subscriptions
    3. Install PanHandler (Version 4.5+) or other skillet-supported applications, such as SLI
    4. Configure the NGFW for IronSkillet

> **NOTE**: You must have IronSkillet configured on your NGFW before loading the eSports solution 
> since many eSports configuration elements depend on IronSkillet elements.

## Submodules Utilized

This quickplay solution uses the [panos-config-elements](https://gitlab.com/panw-gse/tech-library/configure/panos-config-elements) 
repository as a submodule.

## Detailed Description

The eSports panos skillet configures the following elements: 

    * Virtual Wire or L3 deployments
    * QoS prioritization for eSports and eSport streaming applications
    * Tuning rule for day-2 policy optimizer