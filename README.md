### Synopsis

KRPC is simple remote procedure call mechanism used by bittorrent DHT
but might be used anywhere else.

### Description

KRPC basically consisting of bencoded dictionaries sent over UDP. This
implementation provides extra safiety by separation of procedure
signature and implementation and baking procedure type in host
language, thus it's hard to shoot yourself in the foot accidently.

See bittorrent DHT [specification][spec] for detailed protocol
description.

### Example

TODO

#### Modules

* Remote.KRPC — simple interface which reduce all RPC related stuff to
  a few lines. Should be used in the first place.

* Remote.KRPC.Protocol — raw protocol implementation.
* Remote.KRPC.Scheme — message validation.

### Documentation

For usage see examples in ```examples``` directory.
For documentation see haddock generated documentation.

### Build Status [![Build Status][status-img]][status-link]

### Maintainer <pxqr.sta@gmail.com>

Feel free to report bugs and suggestions via github
[issue tracker][issues] or the mail.

[spec]:        http://www.bittorrent.org/beps/bep_0005.html#krpc-protocol
[status-img]:  https://travis-ci.org/cobit/krpc.png
[status-link]: https://travis-ci.org/cobit/krpc
[issues]:      https://github.com/cobit/krpc/issues
