# atomsInMolecule (Python Module)

[![wercker status](https://app.wercker.com/status/ea298b1bcee181efc903b099bc37ad78/m "wercker status")](https://app.wercker.com/project/bykey/ea298b1bcee181efc903b099bc37ad78)

This module provides practical entities to deal with atoms and molecules when comparing various computational chemistry software.


## Testing
```shell
cd tests
py.test -v
```

## Good Practices

Check those links:
- https://pytest.org/latest/goodpractises.html
- http://www.scotttorborg.com/python-packaging/minimal.html
```shell
virtualenv .   # create a virtualenv directory in the current directory
source bin/activate
python setup.py install
pip install --upgrade pip
pip install pytest
##pip install -m requirements-dev.txt
...
```

Make sure that "mypkg" is importable, for example by typing once:
```shell
pip install -e .   # install package using setup.py in editable mode
```

Typically you can run tests by pointing to test directories or modules:
```shell
py.test tests/test_main.py                  # for external test dirs
py.test atomsinmolecule/tests/test_main.py  # for inlined test dirs
py.test atomsinmolecule                     # run tests in all below test directories
py.test                                     # run all tests below current dir
...
```

Don't forget to quit the virtual environment
```shell
deactivate
```

## License

The code which makes up this Python project template is licensed under the MIT/X11 license. Feel free to use it in your free software/open-source or proprietary projects.
