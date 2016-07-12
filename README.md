Simple ansible role, which can be run on `Ubuntu 14.04/16.04` to:
- build netatalk (http://netatalk.sourceforge.net) service from source code
- pack it into .deb archive using checkinstall
- install it on the same system
- create directory and expose it for Time Machine Backups

You will most likely need to adjust configuration (ie. `valid users = ms`).
