VaudTax 2016 package generator
==============================

This is a Debian-package generator for VaudTax 2016.

How to build a Debian VaudTax package
-------------------------------------

1. Make sure to have the following packages installed:

* dpkg-dev
* debhelper (>= 9)
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
    $ quilt push -af
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

All that code is GPLv3+, Copyright 2013-2016, Didier Raboud <didier@raboud.com>.

VaudTax itself is proprietary code owned by the Swiss Vaud canton.
