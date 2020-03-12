# Python Virtual Environment
Notes for python

##Creating a virtual Environment

Creating a virtual environment
venv (for Python 3) and virtualenv (for Python 2) allow you to manage separate package installations for different projects. They essentially allow you to create a “virtual” isolated Python installation and install packages into that virtual installation. When you switch projects, you can simply create a new virtual environment and not have to worry about breaking the packages installed in the other environments. It is always recommended to use a virtual environment while developing Python applications.

On macOS and Linux:
```
python3 -m venv env
```
On Windows:
```
py -m venv env
```
The second argument is the location to create the virtual environment. Generally, you can just create this in your project and call it env.

venv will create a virtual Python installation in the env folder.

## Activating a virtual environment
Before you can start installing or using packages in your virtual environment you’ll need to activate it. Activating a virtual environment will put the virtual environment-specific python and pip executables into your shell’s PATH.

On macOS and Linux:

```
source env/bin/activate
```

On Windows:
```
.\env\Scripts\activate
```

You can confirm you’re in the virtual environment by checking the location of your Python interpreter, it should point to the env directory.

On macOS and Linux:

```
which python
.../env/bin/python
```
On Windows:
```
where python
.../env/bin/python.exe
```

As long as your virtual environment is activated pip will install packages into that specific environment and you’ll be able to import and use packages in your Python application.

Leaving the virtual environment
If you want to switch projects or otherwise leave your virtual environment, simply run:

```
deactivate
```

If you want to re-enter the virtual environment just follow the same instructions above about activating a virtual environment. There’s no need to re-create the virtual environment.
