yenc-freddie 0.3
================

Disclaimer: 

Not my software, just figured I would put it on github, since
it would appear that this is somewhat hard to find.

Use: 

This a fairly simple module, it provide only raw yEnc encoding/decoding with
builitin crc32 calculation.
Header parsing, checkings and yenc formatting are left to you (see examples 
directory for possible implementations). The interface was originally intended 
to be similar to the uu module from Python standard library.
Version 0.2 changed a bit the previous (0.1)  behaviour, but it should be
more usable and flexible (now you can encode/decode from and to standard
input and output and use filenames instead of file objects as arguments
for encode() and decode() ). See CHANGES file for details.
Version 0.3 doesn't introduce anything new, just a bugfix a some internals
changes

good yenc module for use with newsmangler, the yenc-vanilla one included with newsmangler is no good.

```bash
How to install:

1.  python setup.py build
2.  sudo python setup.py install
```
```bash
How to use with newsmangler:
1.  edit newsmangler/newsmangler/yenc.py
2.  change HAVE_YENC_FRED = True
3.  Go to bottom of yenc.py
4.  Change HAVE_YENC_FRED = ('Freddie mod' in _yenc.__doc__)
		to
	HAVE_YENC_FRED = ('Freddie' in _yenc.__doc__)
```bash






For more information check out README-ORIGINAL


