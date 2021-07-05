---
title: "Reports"
weight: 75
---

Welcome to the Reports Page

{{< img src="/Reports/mainreports.png" alt="Dashboard View" >}}

<h1 style="color:black;font-size:20px;">Overview</h1>

The Reports workspace provides an overview of important metrics in your SaltStack Config environment, such as number of licenses available and used, or the Salt version installed on different nodes. You can view reports under the Home screen. Reports update automatically to reflect the current state of your system.

Report data is provided for all minions. However, some reports can be filtered by target group. See Minions for more information.

In the Reports workspace you can download reports in either JSON or CSV format.

<h1 style="color:black;font-size:20px;">Types of Reports</h1>

The SaltStack Config user interface includes several reports to provide an overview of important metrics in your SaltStack Config environment.

Report data is provided for all minions. However, some reports can be filtered by target group.

Minions are nodes running the minion service, which can listen to commands from a Salt controller and perform the requested tasks. A target is the group of minions, across one or many Salt controllers, that a job’s Salt command applies to. A Salt controller can also be managed like a minion and can be a target if it is running the minion service. 