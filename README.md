# Quickplay Solutions Workflow

The Quickplay Solutions workflow provides a one-stop shop for running all use-case specific 
quickplay solutions.

## Solutions Included

The following configuration solutions are included in this workflow:

    * IronSkillet
    * K-12 
    * eSports
    * HomeSkillet
    * Best Practices 

The workflow additionally provides these services:

    * Load an empty, 'out-of-the-box' baseline configuration while saving existing admin credentials and management interface configurations
    * Activate all licenses using an auth-code
    * Perform a threat and anti-virus content update

To read more about each solution included, navigate to the solution's folder, and view
the README.md.

## Using the Workflow

It is assumed that you have PanHandler Version 4.5+ already installed. Follow these instructions for running the Quickplay Solution Workflow:

1. Import this repository into PanHandler
2. Navigate to the *Skillet Collections* page 
3. Click on the **Quickplay Solutions** collection tile
4. Click on the **Quickplay Solution Workflow** tile to run the solution
5. Input your NGFW IP, admin credentials, and PAN-OS software version
6. Input the *Deploy*, *Configure*, and *Assess* sub-skillets you need executed
7. Click **Submit** to start the workflow execution. You will need to input additional information for each sub-skillet executed
8. Continue through the workflow until you reach the *Workflow Completed* page, signifying the end of the workflow

You can additionally run this solution using the SLI Python package. See instructions, [here](https://pypi.org/project/sli/).