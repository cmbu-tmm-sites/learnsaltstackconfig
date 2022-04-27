---
title: "Patching and Updating Windows with SaltStack"
weight: 100
---

<h1 style="color:black;font-size:20px;">Patching and Updating Windows with SaltStack</h1>

This section will go over how to patch and update Windows machines using SaltStack. SaltStack has a comprehensive amount of Windows content and packages that can help Windows administrators with common tasks. SaltStack also provides capabilities to install software on Windows machines using chocolatey or a WinRepo setup in github that is maintainted by SaltStack and the community. The WinRepo makes it easy and simple to get started installing software and creating your own software deployment scripts.

<h1 style="color:black;font-size:20px;">Windows Local Group Policy</h1>
Within SaltStack you can write state files to modify local group policy or handles patching and much more. Lets look at a quick example of a local group policy state file. In SaltStack you can place states in folder /srv/salt or in SaltStack Config in the File Server.

{{< img src="locgrppol.png" width="400" height="500">}}

If you want to create a job to run the state go to the Jobs section of SaltStack Config.

{{< img src="jobwindowspolicy.png" width="400" height="500">}}



