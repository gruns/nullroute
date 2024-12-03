<h1 align="center">
  <img src="prohibited.png" width="260px" height="260" alt="nullroute">
</h1>

## NullRoute

`nullroute` is a small Python script that null routes a host by adding it, and host derivaties like `www.{host}`, to `/etc/hosts`. I use it to quickly null route/block domains I don't want to get distracted by.

Example:
  * You find yourself on https://distracting-website.com/this-page-is-distracting.
  * <30 minutes go by>
  * "That was a waste of time.", you mutter to yourself.
  * Run `sudo nullroute https://distracting-website.com/this-page-is-distracting`.
  * Don't lose 30 minutes on distracting-website.com again.


#### Get Started

First, install `nullroute`'s dependencies:

```
pip3 install furl docopt tld
```

Then download [the script](/nullroute), place it somewhere in your path, and run it with:

```
$ sudo nullroute <urlOrDomain>
```

Example:

```
$ sudo nullroute https://www.marca.com/en/boxing/2024/08/04/66aff511ca4741e8518b45e2.html
Null routed "marca.com" and "www.marca.com" in /etc/hosts.
```

The first and only arguemnt, `<urlOrDomain>`, can be a URL or hostname.


#### License

MIT