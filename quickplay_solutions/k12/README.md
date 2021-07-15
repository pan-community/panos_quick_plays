# K-12 Quickplay Solution

The K-12 Skillet is intended to help enable a safe and secure internet experience. 
The solution hardens a network by building off of the IronSkillet configuration and by enabling 
Safe Search features across the institution without having to manually configure and audit devices.

## Prerequisites 
The following should be completed before running the K-12 Quickplay Solution:

    1. Deploy a PAN-OS 10.X NGFW
    2. License NGFW with the Threat, URL, and WildFire subscriptions
    3. Install PanHandler (Version 4.5+) or other skillet-supported applications, such as SLI
    4. Configure the NGFW for IronSkillet

> **NOTE**: You must have IronSkillet configured on your NGFW before loading the K-12 solution 
> since many K-12 configuration elements depend on IronSkillet elements.

## Submodules Utilized

This quickplay solution uses the [SLED-components](https://github.com/annabarone/SLED-components) repository as
a submodule.

## Detailed Description

The K-12 panos skillet configures the following elements: 

    * Dynamic configuration based on the desired Safe Search deployment:
        * Transparent - SSL inspection with NGFW enforced Safe Search
        * DNS-Proxy - NGFW responds to Google and Bing search engine requests with Safe Search only server IPs
        * Local DNS CNAME - Limits outbound DNS requests to sanctioned internal DNS servers with Google and Bing Safe Search configurations
    * Optional country block: Only allows IPs from US, Mexico, Canada, and cloud providers (based on EDL)
    * K-12 Reports
    * Targeted decryption policies to help enable SSL Decryption adoption and limit risk
    * Chromebook and SAML no-decrypt decryption policies

Additional Safe Search information can be found at: https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-admin/url-filtering/safe-search-enforcement.html
