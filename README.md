# ProTester
Handle c++ projects and testing

### Directories  
/  
|-bin   //Executable files (*.exe)  
|-obj   //Compiled and assembled (not linked) (*.o)  
|-src   //Source code (*.cc)  
|-test  //Tests inputs and outputs (*.in,*.out)  
|-output//Program's output to different tests  

### Workflow
Create a project, add tests and objects and set the includes. Once you do this, just call ``protest`` in your project folder to run tests, compile and/or execute.

### "Hello test"

Execute the following, changing {project_name} for a name of your choice

``protest -n {project_name}``  
``cd {project_name}``  
``protest``  

You should see the template code executing its tests (and hopily passing them)

### Setup

Create a bin folder under your home directory  
``cd``  
``mkdir bin``  

Copy content into the folder:  
bin/  
|-protester  
|-protesterFiles  

And you should be ready to go.  

*Note for pro2 users*: Make sure you defined the $INCLUSIONS env var
### FAQ

**Unrecognized command**  
Is the bin folder in $PATH variable? (echo $PATH)
If not, you should add it. Do this by editing a file usually called .*rc in your home directory (The name of the file can change on different distros)

**Library not found**  
Set the $INCLUSIONS environment var with the path to libraries (in pro2: /assig/pro2/inclusions)

**Class not defined**  
You should add all the objects (.o files (compiled and assembled classes)) to be linked inside obj directory
