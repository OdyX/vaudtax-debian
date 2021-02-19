VaudTax 2020 package generator
==============================

This is a Debian-package generator for VaudTax 2020.

How to build a Debian VaudTax package
-------------------------------------

1. Make sure to have the following packages installed:

* dpkg-dev
* debhelper (>= 13)
* wget
* devscripts
* quilt

2. Download the latest version and prepare the build: run the following
   command from the root of this repository:
<pre>
$ debian/rules get-orig-source
</pre>

3. Apply the patches:
<pre>
    $ QUILT_PATCHES=debian/patches quilt push -af
</pre>

4. Build the binary package:
<pre>
    $ debuild -b
</pre>

5. Install it:
<pre>
# debi
</pre>

LICENSE
-------

All that code is GPLv3+, Copyright 2013-2020, Didier Raboud <didier@raboud.com>.

VaudTax itself is proprietary code owned by the Swiss Vaud canton.
