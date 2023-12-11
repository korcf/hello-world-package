# Example Package

This is a simple example package. View the package at
[GitHub](https://github.com/korcf/hello-world-package)
and
[TestPyPi](https://test.pypi.org/project/hwpkg/).

## Installation

Create a virtual environment
```
$ python3 -m venv .ve
$ source .ve/bin/activate
```

### Options

#### Install from TestPyPI

```
$ pip install -i https://test.pypi.org/simple/ hwpkg
```

#### Install from GitHub

```
$ pip install git+https://github.com/korcf/hello-world-package.git
```

#### Install from a local source tree

```
$ git clone git@github.com:korcf/hello-world-package.git
```
```
$ pip install hello-world-package/
```

#### Install from local distribution archives

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

## Run

Run python in the `.ve` virtual environment
```
$ python
```
and import the package
```
>>> from hwpkg import hello
>>> hello.hello_world()
Hello, World!
```
