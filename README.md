# Python_Notes
Notes for python

## Activating a virtual environment
Before you can start installing or using packages in your virtual environment you’ll need to activate it. Activating a virtual environment will put the virtual environment-specific python and pip executables into your shell’s PATH.

On macOS and Linux:

source env/bin/activate
On Windows:

.\env\Scripts\activate
You can confirm you’re in the virtual environment by checking the location of your Python interpreter, it should point to the env directory.

On macOS and Linux:

```which python
.../env/bin/python
```
On Windows:

where python
.../env/bin/python.exe
As long as your virtual environment is activated pip will install packages into that specific environment and you’ll be able to import and use packages in your Python application.

Leaving the virtual environment
If you want to switch projects or otherwise leave your virtual environment, simply run:

deactivate
If you want to re-enter the virtual environment just follow the same instructions above about activating a virtual environment. There’s no need to re-create the virtual environment.
