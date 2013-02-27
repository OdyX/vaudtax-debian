VaudTax 2012 package generator
==============================

This is a Debian-package generator for VaudTax 2012.

How to build a Debian VaudTax package
-------------------------------------

1. Make sure to have the following packages installed:
* dpkg-dev
* debhelper (>= 9)
* wget
* devscripts

2. Download the latest version and prepare the build: run the following
   command from the root of this repository:
<pre>
$ debian/rules get-build-orig
</pre>

3. Build the binary package:
<pre>
    $ debuild -b
</pre>

4. Install it:
<pre>
# debi
</pre>

LICENSE
-------

All that code is GPLv3+, Copyright 2013, Didier Raboud <didier@raboud.com>.

VaudTax itself is proprietary code owned by the Swiss Vaud canton.
