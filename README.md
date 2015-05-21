# ProTester
Handle c++ projects and testing

### Directories  
/  
|-bin   //Executable files (*.exe)  
|-obj   //Compiled and assembled (not linked) (*.o)  
|-src   //Source code (*.cc)  
|-test  //Tests inputs and outputs (*.in,*.out) or test mains (new protester projects)  
|-output//Program's output to different tests  

### Workflow
Create a project, add tests and objects and set the includes. Once you do this, just call ``protester`` in your project folder to run tests, compile and/or execute.

### "Hello test"

Execute the following, changing {project_name} for a name of your choice

``protester -n {project_name}``  
``cd {project_name}``  
``protester``  

You should see the template code executing its tests (and hopefully passing them)

### Setup

Create a bin folder under your home directory  
``cd``  
``mkdir bin``  

Copy content into the folder:  
bin/  
|-protester  
|-protesterFiles  

And you should be ready to go.  

### FAQ

**Unrecognized command**  
Is the bin folder in $PATH variable? (echo $PATH)
If not, you should add it. Do this by editing a file usually called .*rc in your home directory (The name of the file can change on different distros)

**Library not found**  
Create src/inc in your project, and place there your headers

**Folder doesn't exist**  
Create the folder that doesn't exist and try again

**Class not defined**  
You should add all the objects (.o files (compiled and assembled classes)) to be linked inside obj directory
