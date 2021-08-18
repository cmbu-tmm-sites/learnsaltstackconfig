---
title: "File Server"
weight: 204
---

Welcome to the File Server Page

<img src="fileservermain.png" alt="FileServer" width="700" height="800">

<h1 style="color:black;font-size:20px;">Overview</h1>

The File Server section is where you can create state files to manage your infrastructure. You can post .sls files, scripts, configuration files and files that you may want to distribute to minions. You can also create them in a variety of scripting languages such as YAML, python, json etc. These files can be accessed via jobs or ad-hoc commands from within SaltStack Config. 

The File Server consists of <a href="https://docs.saltproject.io/en/latest/topics/tutorials/starting_states.html">state files</a> that declare the configuration of your infrastructure. 

When you create state files within this section they are stored in the SaltStack Config postgres database. The file server also provides a tree like structure to place files and scripts, then those can be called by other state files. For instance if you have a state file that pushes a configuration file down to a minion the state could look something like this:
<br>
</br>
<img src="/Config/File_Server/samplescriptstate.png">

Basically the line of code above instructs Salt to push that file down and the source starts with salt:// because that points to the <i>base</i> file roots location within the File Server tree structure. You can store config files in the file server then push them down to the minion, or call scripts via <a href="https://docs.saltproject.io/en/latest/ref/states/all/salt.states.cmd.html"><i>cmd.script</i></a> command to locally execute a script that is stored in the File Server.

When you create state files you can then create jobs to run them. Within the Config sections there is a Jobs link where you can go to create jobs. 

If you look at the top of the File Server page you will see a dropdown that points to environments then a path section.<br>
</br>
<img src="/Config/File_Server/fileserverenvpath.png">
<br>
</br>
The dropdown will allow you to choose an environment or you can create your own by typing in a new name. This will allow you to seperate out various environments in how you structure you state files. You may have a Dev section or a Prod section. 

The path is the folder and file name where you want to store the file. So in example above the init.sls file will be created in the /base/apache folder.

You can also run these state files from the CLI on the salt master that is connected to the SaltStack Config via the eAPI Plugin. From the CLI you can run a remote execution commmand to run the state file:

<code>salt '*' state.apply apache test=True</code>

There are some state file examples and tips here as well <a href="https://blogs.vmware.com/management/2021/06/getting-started-with-saltstack-config-part-1-creating-state-files.html">Getting Started with SaltStack Config: State Files Blog</a>

<h1 style="color:black;font-size:20px;">Salt Environments</h1>

One thing you will notice in the interface is a dropdown with two defaults environemtns: <i>base</i> and <i>sse</i>. The <i>base</i> environment is essentially the default "file_roots" location for SaltStack Config. In otherwords this is where the system will look for files by default (ex. top files, when source is salt://). You can also create your own environments by simply typing in a custom environment name into the dropdown field and pressing enter. <br>
<br>
<img src="/Config/File_Server/envdropdown.png" width="600" height="700">
<br>
Creating custom environments can be useful if you want to seperate out workstreams or just organize your state files more logically. Also if you want to execute a state file from the CLI and that state file is not in base then you will need to specify the environment.

<code>salt '*' state.apply apache saltenv=dev test=True</code>

The path section is just the folder and name of the file you are creating. You can either create a new directory or create a file that will go into an existing directory. <br>
<br>
<img src="/Config/File_Server/pathsection.png" width="500" height="600">
<br>
Then the file would be located in the /opencart/files directory.
<br>
<br>
<img src="/Config/File_Server/treestruct.png" width="250" height="450">
<br>
<br>
<h1 style="color:black;font-size:20px;">Accessing the State Files</h1>
<br>
Once you have created the state files in the file server, you can access them for execution using a couple of methodologies. One way is to create jobs that call the states, you can learn more about jobs here. Admins can also call these state files via the CLI like you see above on this page. 
