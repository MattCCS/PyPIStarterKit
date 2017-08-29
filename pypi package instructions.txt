1) mkdir <DIR>; cd <DIR>
2) mkdir <name>
	a) touch <name>/__init__.py
	b) touch <name>/main.py
3) touch README.md (make Markdown- and ReST-common)
4) echo "include README.md" >> MANIFEST.in
5) (create setup.py)


Registering on GitHub:
0) (create project on GitHub)
1) git init .
2) graome <name>
3) (git ignore)
4) (commit + push)
	5) (gpohi if initial)
5) (verify + tag + push)


Registering on PyPI:
1) pypireg [test/live] (from top of project)


Uploading to PyPI:
1) pypiup [test/live] (from top of project)


Testing on PyPI:

	Testing (local):
	1) pip3 install -e .
	2) pip3 uninstall <name>

	Testing (test):
	1) pip3 install <name> -i https://testpypi.python.org/pypi
	2) pip3 uninstall <name>

	Testing (live):
	1) pip3 install <name>
	2) pip3 uninstall <name>


Parting thoughts:
-----------------
- don't care about bdist crap -- 2 and 3 are different
