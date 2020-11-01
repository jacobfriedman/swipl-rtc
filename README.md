# swipl-rtc

This package enables Prolog to interface with [libdatachannel](https://github.com/paullouisageneau/libdatachannel). Linux & WASM Architectures aim to be supported.

## Installation

```
?- pack_install('file:///home/<user>/<clone directory>').
```

*Note: .git DL not working yet...*
```
?- pack_install('https://github.com/jacobfriedman/swipl-rtc.git').
# yields:
ERROR: Domain error: `pack_name' expected, found `'swipl-rtc''
ERROR: In:
ERROR:   [14] throw(error(domain_error(pack_name,'swipl-rtc'),_21064))
ERROR:   [11] prolog_pack:pack_default_options('https://github.com/jacobfriedman/swipl-rtc.git','swipl-rtc',[],_21106) at /usr/local/lib/swipl/library/prolog_pack.pl:494
ERROR:   [10] prolog_pack:pack_install('https://github.com/jacobfriedman/swipl-rtc.git') at /usr/local/lib/swipl/library/prolog_pack.pl:457
ERROR:    [9] toplevel_call(user:user: ...) at /usr/local/lib/swipl/boot/toplevel.pl:1113
ERROR: 
ERROR: Note: some frames are missing due to last-call optimization.
ERROR: Re-run your program in debug mode (:- debug.) to get more detail.
```
## Example Usage
## Api Overview
Api documentation can be found ____.
---

## Tests
### Building 
Rather than build in-package (we want to build for the WASM & Docker Envs without make), 
we suply the libdatachannel library shared object. We build with GnuTLS

```
apt-get install -y \
	gnutls-bin \
	libsrtp2-dev 
```
from [libdatachannel](https://github.com/paullouisageneau/libdatachannel).

* NOTE: WASM BUILD *

Need to test the static archive .a to see if it works with the wasm.


### Running
### Changelog
- *0.0.2*
	Added in wasm-emscripten .a output
	Included linked .so
- *0.0.1*
	Created Library

### Known Issues
### Licence 

Please see the LICENSE file included with this package.

### Contributors / Credit

- *Jaschen Duschletta* for the inspiration and direction
- *Raavio Laanemets* for SWIPL-WASM work
- *Jan Wielemaker* for maintenance of the SWIPL Library

