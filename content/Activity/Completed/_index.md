---
title: "Completed"
weight: 20
---

Welcome to the Completed Activities Page

{{< img src="/Activity/Completed/completedmain.png" alt="Completed Activities" >}}

<h1 style="color:black;font-size:20px;">Overview</h1>

Completed Activity section can be used to monitor the status of completed jobs or activities. There are various status codes you may see on this page under the Status column:

<b>Completed</b> - the job has finished<br>
<b>Partial</b> - the job is still waiting for some minions to return data<br>
<b>Skipped</b> - the job was scheduled but did not run<br>
<b>Disabled</b> - the job is part of a disabled schedule<br>
<b>Stopped</b> - the job was stopped and cannot be resumed<br>
<b>Failed</b> - the job ran but failed on the minion(s)<br>

You can view the return data from the executed jobs by clicking on the JID link in the associated jobs column. When you click on the JID you will be presented with the return data in a couple of different formats. If you did a state.apply for instance you will see highdata being returned.

{{< img src="/Activity/Completed/highstatereturn.png" alt="Highstate Return">}}

There is also a way to view the Raw JSON response. This can be helpful in troubleshooting and/or looking at what happened on the Event Bus.

{{<img src="/Activity/Completed/rawdatareturn.png" alt="Raw Data Return">}}




