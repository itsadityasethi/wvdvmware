# Exercise 3: Deploying a Farm

## About Farm Deployment

A farm is a collection of Microsoft Remote Desktop Services (RDS servers) on Microsoft Azure that host applications and desktops. Farms simplify RDS host management because you can use farms to serve multiple user subsets where the sizes of the subset vary, or the desktop or application requirements vary. Farms can provide session-based desktops and remote applications.

Ideally, you provide the resources that users need to do their jobs without delays, and at the same time, avoid the cost of unused resources that are powered on but sitting idle. Horizon Cloud Service provides power management capabilities for the Microsoft Azure servers so hosts are automatically powered hosts on and off and deallocated, as needed. The result is that farms can automatically scale out to the maximum size when necessary, and scale down to minimum size when not needed. This reduces cloud capacity costs, as well as computing costs for deallocated servers.

You set up these options in the Horizon Cloud Service farm profile when you first create the farm, and you can also modify the settings at any time afterward.

**Note:** For this set of exercises, you need a server image deployed.

## Exercise 3.1: Creating a Farm

When the new image has been published, you can use it to create farms.

### Task 1: Create a New Farm



In the navigation bar of Horizon Cloud Service Administration Console, select Inventory.
Select Farms.
In the Farms window, click New.

### Task 2: Provide General Settings


1. In the New Farm window, **Definition** tab, provide the following information, and then scroll down.
  - **Name:** Enter a name to help identify this farm in the system.
  - **Description:** Enter an optional description to help identify the farm in the system.
  - **VM Names:** Enter a name for all server VMs created for this farm to which a number is appended, such as win2016-1, win2016-2, and so on. The name must start with a letter and can contain only letters, dashes, and numbers.
  - **Farm Type:** Specify the type of asset this farm provides to end users. Keep this assignment time in mind when you select the server size, since desktop assignments may require more capacity.
Desktops: Provides session-based desktops
Applications: Provides access to remote applications
Location: Select the location from the list of pods in the pop-up menu.
Pod: Select the pod for this farm.
Scroll down to provide additional general settings.
