# PyPI Packaging Instructions
PyPI is the [Python Package Index](https://pypi.python.org/pypi).


## 1 - Project Setup
1. `mkdir <DIR>; cd <DIR>`
2. `mkdir <name>`
    1. `touch <name>/__init__.py`
    2. `touch <name>/main.py`
3. `touch README.md` (make Markdown- and ReST-common)
4. `echo "include README.md" >> MANIFEST.in`
5. (create `setup.py`)


## 2 - Registering on GitHub
1. (create project on GitHub)
2. git init .
3. graome <name>
4. (git ignore)
5. (commit + push)
6. (verify + tag + push)


## 3 - Registering on PyPI
1. pypireg <test/live> (from top of project)


## 4 - Uploading to PyPI
1. pypiup <test/live> (from top of project)


## 5 - Testing on PyPI

### Local
1. pip3 install -e .
2. pip3 uninstall <name>

### Test
1. pip3 install <name> -i https://testpypi.python.org/pypi
2. pip3 uninstall <name>

### Live
1. pip3 install <name>
2. pip3 uninstall <name>


## Parting thoughts
- don't care about bdist crap -- 2 and 3 are different
