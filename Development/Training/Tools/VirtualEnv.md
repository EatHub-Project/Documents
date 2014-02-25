# VirtualEnv
VirtualEnv is a tool created to isolate Python environments. 

The basic problem being addressed is one of dependencies and versions, and indirectly permissions. Imagine you have an application that needs version 1 of LibFoo, but another application requires version 2. How can you use both these applications? If you install everything into /usr/lib/python2.7/site-packages (or whatever your platform’s standard location is), it’s easy to end up in a situation where you unintentionally upgrade an application that shouldn’t be upgraded.

This will be useful for our development as we can be sure that all the team members have the same libraries, the same versions, and don't have any other external dependencies that might interfere. 

We will install all the packages needed for our project under a VirtualEnv, and share a common requirements.txt to easily setup the environment with pip.

## Instalation

### Windows

### Linux

### OSX


## Usage


### Initialize

The basic usage is:

```
$ virtualenv venv
```
This creates ```ENV/lib/pythonX.X/site-packages```, where any libraries you install will go. It also creates ```ENV/bin/python```, which is a Python interpreter that uses this environment. Anytime you use that interpreter (including when a script has #!/path/to/ENV/bin/python in it) the libraries in that environment will be used.

It also installs Setuptools (pip) into the environment.

### Activate

In a newly created virtualenv there will be a ```bin/activate``` shell script. For Windows systems, activation scripts are provided for CMD.exe and Powershell.

On Posix systems you can do:

```
$ source venv/bin/activate
```

This will change your $PATH so its first entry is the virtualenv’s ```bin/``` directory. 

This way, packages will be instaled to and used from the ```bin/``` directory, instead of the system's. 

### Windows Notes
Some paths within the virtualenv are slightly different on Windows: scripts and executables on Windows go in ```ENV\Scripts\``` instead of ```ENV/bin/``` and libraries go in ```ENV\Lib\``` rather than ```ENV/lib/```.

To create a virtualenv under a path with spaces in it on Windows, you’ll need the [win32api](http://sourceforge.net/projects/pywin32/) library installed.

## References
- [VirtualEnv docs](http://www.virtualenv.org/en/latest/virtualenv.html)