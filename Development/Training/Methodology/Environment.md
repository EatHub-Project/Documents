# Development environment 

In this document we describe how to setup and manage the environment for development.

## Setup

1. **Install Python and VirtualEnv**: The first thing to do is make sure you have *Python 2.7* installed in your machine. Then, install *pip* and *VirtualEnv* as detailed in their respective documents.

2. **Install MongoDB**: ... **[this process is incomplete yet]**


3. **Clone the repository**: Next thing is to get the source code from the main repository. For that you just need to clone the remote repository to a local directory, either from command line or SourceTree.

4. **Activate VirtualEnv**: From the command line, initialize and activate a *VirtualEnv* in the project root directory. Then, activate it. Instructions are provided in VirtualEnv's document.

5. **Install project dependencies**: The source code includes a *requirements.txt* file with all the package dependencies. Downlaod and install them with *pip* as specified in pip's document. It's just 1 command.

6. **Load database data**: For development purposes, testing data for the database will be provided as the project evolves. Load it to your local MongoDB database. **[this process is incomplete yet]**

6. **Test**: Make sure everything is fine. Run the project to check that it works as spected. If you are using the master branch of the repository, you should have a *stable* version running. If you are using the development branch, the project can be unstable, but it should at least be able to run. Status in other branches is indeterminated.


## Making changes

During development you might need to modify either package dependencies or database information. These changes are special, because other members of the team need to take action upon them.

Every time you change any of these, **make sure** you specify it in your commits and in your *Pull Request*, and also make sure the development lead notices it, so he can inform the rest of the team.

#### Changing database data

If you need to add, remove or modify the data in the database during the development, make a copy and submit them to the source repository. **[this section is incomplete]**

#### Changing dependencies

If you modify any project dependencies, that is, add, remove or modify any packages to your environment, you need to save those changes to the repository.

Before you install anything, you make sure you are in the *VirtualEnv*. After you have done all the operations with the dependencies, you save them to the *requirements.txt*. You can do this with pip or by hand, **but be aware** that doing ```pip freeze``` can return a different result than the lines in the current *requirements.txt* (for instance, giving the package name instead of its repository address), and you should not override these lines.


## Applying changes

When other members of the team make changes to the database or the dependencies, you need to update them manually.

#### Updating the database
**[this section is incompleted]**

#### Updating dependencies
If there are changes in the dependencies, you have to update them with pip. Usually these changes will be updates, so you just need to run ```pip install -r ./requirements.txt```. Other kinds of changes will be explained here if needed.