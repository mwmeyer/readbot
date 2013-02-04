readbot
=======

*A delightful python OCR module*

This is a simple module for adding quick and easy OCR processing within your python program. In addition to wrapping an OCR engine (currently, only [Tesseract](http://code.google.com/p/tesseract-ocr/)) it also handles file input quite liberally. Valid file input may be a string of a files path, a file object, or even a URL to a file on the web. As an added bonus, if you need to perform OCR on a PDF, this module will use GhostScript to convert the file to a PNG for Tesseract.

This module is intended for very basic OCR use and is in no way comprehensive. Right now, it is less than 100 LOC and simply calls a Tesseract subprocess.

Installation
============

Its on pypi!

```shell
$ pip install tesseract
```s

**Tesseract**

You need Tesseract to use this module.

(mac)
```shell
$ brew install tesseract
```

(linux)
```shell
$ sudo apt-get tesseract-ocr
```

Usage
=====

```python
from readbot import ReadBot

rb = ReadBot()

print rb.interpret('/path/to/file/Hello_World.png')
```


