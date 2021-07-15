# IronSkillet Quickplay Solution

IronSkillet is a day one deployment-agnostic NGFW and Panorama configuration. It is used
as an initial baseline including device hardening and security profiles to be used by use-case
specific configuration and security policies.

## Prerequisites 
The following should be completed before running the IronSkillet Quickplay Solution:

    1. Deploy a PAN-OS 10.X NGFW
    2. License NGFW with the Threat, URL, and WildFire subscriptions
    3. Install the latest PanHandler (Version 4.5+) or other skillet-supported applications, such as SLI

## Submodules Utilized

This quickplay solution uses the [ironskillet-components](https://github.com/PaloAltoNetworks/ironskillet-components) 
repository as a submodule.

## Detailed Description

Additional information about the IronSkillet solution can be found on its
[documentation page](https://iron-skillet.readthedocs.io/en/docs_master/).