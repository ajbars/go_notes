# Jenkins CICD learning notes

## Terminal useful notes
:::<terminal usage notes>
In order to run a Jenkins pipeline on GitLab you have to:
1. Best of all, first create a test branch on your repo 
2. Create a file called Jenkinsfile (no extension, with a capital J)
3. Install a GitLab plugin in Jenkins and connect it to the GitLab

I had several problems running the pipeline, will try to list them as well as the stuff I learned that is working

1. Depending on the infrasctructure you may run into a problem setting an agent for a pipeline and at all, choosing the approach. I initially wanted to use the Blue Ocean GUI, but now I just use the standard interface since it's a little bit more informative.
2. I had to use the agent that was provided by my company
3. I wasn't able to install plugins, only ask a devops from a remote infrastructure team to do that, and he refused to install a Go plugin.

`echo "chassis" > car.txt` &nbsp;&nbsp;&nbsp; *Replaces what was in the file with "chassis"*  
`echo "chassis" >> car.txt` &nbsp;&nbsp;&nbsp;*Appends "chassis" to what is already there*  
`grep "chassis" car.txt`   &nbsp;&nbsp;&nbsp; *Searches for "chassis" inside car.txt*  

:::



