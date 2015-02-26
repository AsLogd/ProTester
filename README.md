# ProTester
Handle c++ projects and testing

### Directories
/
|-bin   //Executable files (*.exe)
|-obj   //Compiled and assembled (not linked) (*.o)
|-src   //Font code (*.cc)
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

You should set an environment variable called $INCLUSIONS containing a path to libraries (pro2)

Create a bin folder under your home directory
``cd``  
``mkdir bin``  

Copy content into the folder:
bin/
|-protester
|-protesterFiles

And you should be ready to go.

### FAQ

*Unrecognized command*
Is the bin folder in $PATH variable? (echo $PATH)
If not, you should add it. Do this by editing a file called .**rc in your home directory (The name of the file differs depending in your distro)
