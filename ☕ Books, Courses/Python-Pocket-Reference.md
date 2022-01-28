# Python Pocket Reference, 5th Edition

### Python Command line Usage

Command lines used to launch Python programs from a system
shell have the following format:

`python [ option* ] [ scriptfile | -c command | -m module | - ] [arg*]`

Command-line options intended for Python itself appear before the specification of the program code to be run (option). Arguments intended for the code to be run appear after the program specification (arg)

### Command-Line Program Specification

- To check all available command-line option in python
	- `python -h`
	- print version `python -V` | `python --version`
- **scriptfile**: Denotes the name of a Python script file to run as the main
	- `python main.py`
- **-c command**: Specifies python code as a string to run. `sys.argv[0]` is set to `-c`
	- `python -c "print('Hello, World')"`
- **-m module**: Runs a module as a script: searches for module on `sys.path` and runs it as a top-level file (`python -m pdb s.py` runs the Python debugger module pdb located in a standard library directory, with argument `s.py`). module may also name a package (idlelib.idle). `sys.argv[0]` is set to the module’s full path name.
- **-** : Reads Python commands from the standard input stream, stdin (the default); enters interactive mode if stdin is a “tty” (interactive device). `sys.argv[0]` is set to '−'.
- **arg**: anything else on the command line is passed to the script file or command, and appears in the built-in list of strings `sys.argv[1:]`

### Built-in Types and Operators













