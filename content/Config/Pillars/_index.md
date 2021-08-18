---
title: "Pillars"
weight: 203
---

Welcome to the Pillars Page!

<img src="/Config/Pillars/mainscreenpillar.png">

The Pillars workspace allows you to create and manage pillar data that is stored in SaltStack Config. Pillars are sets of data defined in Salt and passed through to minions. This allows confidential and targeted data to be securely sent only to relevant minions. 

Pillar data is encrypted in the SaltStack Config database and is not stored in plain text. It is also encrypted during transmission. 

Pillar data is written in json when using this pillar workspace.

You can also add in-line pillar data to individual jobs, the jobs section contains more information about that. Sometimes you may want to pass pillar data only when a certain job is run. The Pillar data in the Pillars workspace can be called by state files across the tree structure.

An example of how a state file can call pillar data is below. Basically the state file sets a variable that will be populated with the value of pillar then a for loop is used to iterate over the list.

<img src ="/Config/Pillars/statefilecallpillar.png">



