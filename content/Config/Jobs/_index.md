---
title: "Jobs"
weight: 201
---

<img src="/Config/Jobs/mainjobpane.png" width="900" height="1000">

<h1 style="color:black;font-size:20px;">Overview</h1>

Jobs are used to run remote executions and state files against minions. From the jobs section you can create, configure, save jobs that can be re-run and reused. For example you could have a job that configures a firewall settings on a Linux minion and installs some applications, this job could be run every time a machine is deployed to ensure the same set of applications are installed.

This is also one of the areas of the product where you can run a job and identify a Target group of minions to run the job against. Lets look a bit more on how to create a job.


<h1 style="color:black;font-size:20px;">Create a Job</h1>

<img src="/Config/Jobs/createjobwizard.png" width="500" height="600">

When you go into the jobs section you can create jobs by clicking the Create Job button. You can define the job settings with the following options:

<b>Name</b> - Enter a name for the job<br>
<b>Description</b> - Enter a description (optional)<br>
<b>Command</b> - choose from the following two options:
    <p style="text-indent: 25px;">
       <b>salt</b>: define a job to run on a target group of minion(s)<br></p>
    <p style="text-indent: 25px;">
       <b>salt-run</b>: define a job to run on a Salt master or group of Salt masters</p><br>
<b>Targets</b>- choose a target group of minions to run the job against. This is optional and may be used only if you know which minions you want the job to run against. If you are planning to run this job against random minions in the future then you can leave this blank then run the job against a particular minion in the Minions section.<br>
<b>Function</b>- enter a function to define what the job will do. An example could be <code>state.apply</code> which would run a state file when the job is exectuted.<br>
<b>Arguments</b> - some functions will require arguments. For example the function <code>cmd.run</code> would require arguments to define the command you want to run on the minion.



