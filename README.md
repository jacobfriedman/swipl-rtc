# swipl-rtc

This package enabled Prolog to interface with [libdatachannel](https://github.com/paullouisageneau/libdatachannel).

You may install this pack on swi-prolog by running

```
?- pack_install('https://github.com/<owner>/<pack>.git').
```

## Example Usage

## Api Overview

Api documentation can be found ____.

---

## Tests

### Building 

Rather than build in-package (we want to build for the WASM & Docker Envs without make), 
we suply the libdatachannel library shared object. We build with GnuTLS

Our build uses 
```
apt-get install -y \
			gnutls-bin \
			libsrtp2-dev 
```

[libdatachannel](https://github.com/paullouisageneau/libdatachannel)



### Running

### Changelog

- *0.0.1*
	Created Library

### Known Issues

### Licence 

Please see the LICENSE file included with this package.

### Contributors / Credit

- *Jaschen Duschletta* for the inspiration and direction
- *Raavio Laanemets* for SWIPL-WASM work
- *Jan Wielemaker* for maintenance of the SWIPL Library

