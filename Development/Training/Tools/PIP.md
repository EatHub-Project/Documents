# pip
*pip* is a simple a tool for installing and managing python packages.

Packages can be installed through the command line, either from PyPi *(the official Python Package Index)*, third party repositories, or from a custom source such as a file or a URL.

Additionally, pip allows to use **dependency specification files**, commonly named *requirements.txt*, where dependency packages can be listed to install all of them with one command.

## Installation


## Usage examples

- Install most recent package from PyPi:

```
$ pip install Django
```

- Install package version from a *downloads page*:

```
$ pip install -f http://dist.plone.org/packages/ 'Pillow==1.7.3'
```

- Install from third party repository:

```
$ pip install -i http://pypi.ejemplo.com/simple SQLObject
```

- Install from source code:

```
$ pip install http://ejemplo.com/ruta/a/MiPaquete-1.2.3.tgz
```

- Install a specific version of a package:

```
$ pip install 'ZopeSkel==2.21.2'
```

- Install from a *requirements.txt* file:

```
$ pip install -r ./requirements.txt
```

With the following content in requirements.txt:

```
python-ldap
django
buildbot
buildbot-slave
PyYAML
south
```

- Write current dependencies into a file:

```
pip freeze > requirements.txt
```

## References
- [pip official webpage](https://pypi.python.org/pypi/pip)
- [Distribute and pip (in Spanish)](http://lcaballero.wordpress.com/2013/03/20/instalacion-de-paquetes-python-con-distribute-y-pip/)