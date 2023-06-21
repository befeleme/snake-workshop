# Installing Python for Windows

If you have Windows 10 with the latest updates, enter `python3` in the command line.

If you don't have Python installed yet, the Microsoft Store page will automatically open for you. Install Python from there.

If you already have Python installed, something like this will appear in the command line:


```plain
> python3
Python 3.8.1 (...)
Type "help", "copyright", "credits" or "license" for more information.
>>>
``` 

On the first line of the output is the version of Python. Check that the version is 3.6 or newer (for example, `Python 3.6.10`, `Python 3.7.4` or `Python 3.8.1`). 
If it is, you have Python installed!
End it with the shortcut <kbd>Ctrl</kbd>+<kbd>Z</kbd> and <kbd>Enter</kbd> so that the line where you will write further commands does not start with "three beaks" (`>>>`).
<br><!-- instructions in case the window is accidentally closed: -->
(Or close the window with the command line. When you need it again, you can open a new one.)

If you did not get the output above, or the versoin is too low, continue with the section below.


## Older Windows or existing Python

If the shortcut `python3` doesn't work or if you have an older version of Python, go to the [download page](https://www.python.org/downloads/) and download the installer for the latest stable version of Python.
Make sure it is version **3.6.0 or newer** - version 3.6.0 has certain improvements that we will be using in this course.

How to recognize which installer is the right one?
If your computer has a 64-bit version of Windows,
download the *Windows x86-64 executable installer*.
If you have an older computer with 32-bit Windows,
download the *Windows x86 executable installer*.
(The difference is in *x86-64* versus *x86*.)

> [note]
> Where can you find out if you have 32-bit or 64-bit Windows?
>Open the **Start** menu, search for "System," and open **System Information**.
>If you have a newer computer, you almost certainly have 64-bit Windows.
>
>{{ figure(
    img=static('windows_32v64-bit.png'),
    alt='Screenshot of system version check',
) }}

Run the downloaded installer. At the beginning of the installation, check **Install launcher for all users** and also **Add Python to PATH**.
These options will simplify the creation of a virtual environment for you.

(If you don't have administrator privileges, do not check the option *Install launcher for all users*.)

{{ figure( img=static('windows_add_python_to_path.png'), alt='Screenshot instalace Pythonu', ) }}

Then press **Install now** and follow the instructions.

If you have an open command line, close it after installing Python and open a new one.
The installation changes system settings that need to be reloaded.
