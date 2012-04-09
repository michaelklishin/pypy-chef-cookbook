# PyPy Chef Cookbook

This is an OpsCode Chef cookbook for PyPy.

It uses [PyPy Team Ubuntu PPA](https://launchpad.net/~pypy/+archive/ppa) to provide stable PyPy releases (currently 1.8).


## PyPy Version

This cookbook currently provides PyPy 1.8.x but as new releases are pushed to the PPA, they will
be used instead.


## Supported OS Distributions

Ubuntu 10.04, 11.04, 11.10.


## Recipes

Main recipe is `pypy::ppa`.


## Attributes

There are no attributes to tune at the moment.


## Dependencies

 * `apt` cookbook from OpsCode


## Copyright & License

Michael S. Klishin, Travis CI Development Team, 2012.

Released under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.html).
