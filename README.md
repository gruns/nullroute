## NullRoute

#### Overview

`nullroute` is a small Python 3 script that null routes a host by adding it, and host derivaties like `www.{host}`, to /etc/hosts.


#### Get Started

First, install the dependencies:

```
pip3 install furl docopt tld
```

Then download [the script](/nullroute), place it somewhere in your path, and run it with:

```
$ nullroute <urlOrDomain>
```

Example:

```
$ nullroute https://www.marca.com/en/boxing/2024/08/04/66aff511ca4741e8518b45e2.html
Null routed "marca.com" and "www.marca.com" in /etc/hosts.
```

The first and only arguemnt, `<urlOrDomain>`, can be a URL or hostname.


#### License

MIT