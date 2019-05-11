To release a new version, run:

```
bumpversion minor setup.py ecc/__init__.py
```

Options for the first argument are `major`, `minor`, or `patch`.

Then, build a new wheel:

```
python setup.py sdist bdist_wheel
```

Finally, upload to PyPi using Twine:

```
twine upload dist/*
```
