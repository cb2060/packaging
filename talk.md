<script type="text/javascript"
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
# Packaging and documentation

CB2060 Applied programming for life sciences

KTH

---
layout: false

## Goal



## Preparing your package for pypi

A simple tool: flit

* Install flit in your virtual environment

```
(myenv) $ pip install flit
```

Three steps

1. flit init
2. flit build
3. flit publish

---

## init

~~~
$ flit init
~~~

* Answer questions
* generates standars License file
* a `pyproject.toml` file - meta-data about your project

---

## build

~~~
$ flit build
~~~

* Creates a dist subfolder
    - a compressed archive of your source
    - a "wheel", a standardised (binary) zip file with metadata


---

## publish

~~~
$ flit publish
~~~

...and it is available to anyone

---
## Readthedocs/sphinx

* A standard for documenting Python programs
* Documentation published at project.readthedocs.io
* Sphinx tool for generating docs


---

## Initialize

~~~
$ mkdir docs
$ cd docs
$ sphinx-quickstart
~~~

Files generated

* index.rst (the main document)
* conf.py (configuration)


---

## Extract source documentation

~~~
$ cd ..
$ sphinx-api -o docs .
~~~
