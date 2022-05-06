---
title: "Patching and Updating Windows with SaltStack"
weight: 805
---

<h1 style="color:black;font-size:20px;">Patching and Updating Windows with SaltStack</h1>

This section will go over how to patch and update Windows machines using SaltStack. SaltStack has a comprehensive amount of Windows content and packages that can help Windows administrators with common tasks. SaltStack also provides capabilities to install software on Windows machines using chocolatey or a WinRepo setup in github that is maintainted by SaltStack and the community. The WinRepo makes it easy and simple to get started installing software and creating your own software deployment scripts.

<h1 style="color:black;font-size:20px;">Windows Local Group Policy</h1>

Within SaltStack you can write state files to modify local group policy or handles patching and much more. Lets look at a quick example of a local group policy state file. SaltStack allows you to place states in a folder /srv/salt or in SaltStack Config in the File Server.

There are various examples here on how to create state files.
https://docs.saltproject.io/en/latest/ref/states/all/salt.states.win_lgpo.html

If you want to create a job to run the state go to the Jobs section of SaltStack Config.

{{< img src="jobwindowspolicy.png" width="400" height="500">}}

<h1 style="color:black;font-size:20px;">Windows Patching & Updates</h1>

SaltStack has a module for managing Windows Updates using the Windows Update Agent. Use the <a href="https://docs.saltproject.io/en/latest/ref/modules/all/salt.modules.win_wua.html">win_wua</a> modules to get a list of available patches and ensure that they are installed. Below is an example of a state file using either a GUID or KB to determine if the patch is installed.


{{< img src="statefilepatch.png" width="400" height="500">}}

The functions commonly used with win_wua are:

- win_wua.get
- win_wua.download
- win_wua.install
- win_wua.uninstall

