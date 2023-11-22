# Example Package

This is a simple (hello world) example package.

## Installation

Create a virtual environment
```
$ python3 -m venv .ve
$ source .ve/bin/activate
```

### Install from the TestPyPI index

```
$ pip install --index-url https://test.pypi.org/simple/ --no-deps hwpkg
```

### Install from GitHub

```
$ pip install git+https://github.com/korcf/hello-world-package.git
```

### Install from a local source tree

```
$ git clone git@github.com:korcf/hello-world-package.git
```
```
$ pip install hello-world-package/
```

### Install from local distribution archives

```
$ git clone git@github.com:korcf/hello-world-package.git
$ cd hello-world-package/
```
Generate distribution packages
```
$ pip install --upgrade build
$ python -m build
```
Install either from the built distribution
```
$ pip install dist/hwpkg-0.0.1-py3-none-any.whl
```
or from the source distribution
```
$ pip install dist/hwpkg-0.0.1.tar.gz
```
