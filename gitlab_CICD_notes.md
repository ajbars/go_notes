# GitLab CICD learning notes

## Terminal useful notes
:::<terminal usage notes>

ifkonfig command gets ip addresses from the terminal

oh my zsh has very useful kubectl abbreviations. It has to be install on top of the zsh terminal, which is similar to bash

`echo "chassis" > car.txt` &nbsp;&nbsp;&nbsp; *Replaces what was in the file with "chassis"*  
`echo "chassis" >> car.txt` &nbsp;&nbsp;&nbsp;*Appends "chassis" to what is already there*  
`grep "chassis" car.txt`   &nbsp;&nbsp;&nbsp; *Searches for "chassis" inside car.txt*  

:::

:::<CI file structure>
## How to write a CI yaml file
Write a file called gitlab-ci.yml, it will be detected automatically and the jobs in it will be run

### Structure of the file:

`stages:`  
&nbsp;&nbsp;`- build`  
&nbsp;&nbsp;`- test`&nbsp;&nbsp;&nbsp;&nbsp;*//&nbsp;Here are the stages defined, they will be executed consecutively*  
`build the car:`&nbsp;&nbsp;&nbsp;&nbsp;*// name of the job*  
&nbsp;&nbsp;`stage: build`&nbsp;&nbsp;&nbsp;&nbsp;*// In which stage it is to be executed*  
&nbsp;&nbsp;`script:`&nbsp;&nbsp;&nbsp;&nbsp;*// here comes the bash script for this job*  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`- mkdir build`  
...  
&nbsp;&nbsp;`artifacts`:&nbsp;&nbsp;&nbsp;&nbsp;*// what to do with the artifacts*  
&nbsp;&nbsp;&nbsp;&nbsp;`paths:`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`- build`/&nbsp;&nbsp;&nbsp;&nbsp;*// The path to the artifacts folder*  
<br>
`test the car:`  
&nbsp;&nbsp;`stage: test`   
&nbsp;&nbsp;`script:`  
&nbsp;&nbsp;&nbsp;&nbsp;` - test -f build/car.txt`&nbsp;&nbsp;&nbsp;&nbsp;*// Tests whether there is a file with that name inside that folder*  
&nbsp;&nbsp;&nbsp;&nbsp;`- cd build`  
&nbsp;&nbsp;&nbsp;&nbsp;`- grep "chassis" car.txt`  
  
  
If all the commands in the script are successful (for example the grep command finds what we were searching for) , then the job is finished successfully








:::