# PyPy Chef Cookbook

This is an OpsCode Chef cookbook for [PyPy](http://pypy.org).

It uses official tarballs or [PyPy Team Ubuntu PPA](https://launchpad.net/~pypy/+archive/ppa) to provide stable PyPy releases (currently 1.9 from the tarball and 1.8 via the PPA).


## PyPy Version

`pypy::tarball` provides 1.9 by default with an option to change the version via node attributes.

For the PPA flavor, this cookbook currently provides PyPy 1.8.x but as new releases are pushed to the PPA, they will be used instead.


## Supported OS Distributions

Ubuntu 10.04, 11.04, 11.10 for `pypy::ppa`.

Ubuntu 10.04, 11.04, 11.10, 12.04 and any recent Debian release for `pypy::tarball`.


## Recipes

Main recipe is `pypy::tarball`. There is also Main recipe is `pypy::ppa` that uses [PyPy Team Ubuntu PPA](https://launchpad.net/~pypy/+archive/ppa).


## Attributes

For `pypy::tarball`:

 * `node[:pypy][:tarball][:version]` (default: `"1.9"`): PyPy version to install
 * `node[:pypy][:tarball][:installation_dir]` (default: `"/usr/local/pypy"`): where to install PyPy

There are no attributes to tune at the moment for `pypy::ppa`.


## Dependencies

 * `apt` cookbook from OpsCode


## Copyright & License

Michael S. Klishin, Travis CI Development Team, 2012.

Released under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.html).
