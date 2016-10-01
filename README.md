# Isolinear Chips #

This project aims to be the complete network protocol specification
for the game [Artemis Spaceship Bridge
Simulator](http://artemis.eochu.com/). This is a completely unofficial
work, made by fans of the game, spending countless hours reverse
engineering the network protocol.

## Specification format ##

The protocol is specified in the **Simple Type Format** (`.stf`)
format. The format is quite easy for humans to read, but is a
machine-parsable format!

Having a machine-readable protocol specification, makes it possible to
generate protocol parsers (for multiple programming langauges),
analysis tools, and reference documentation, from the same data
source. This prevents the various protocol-related works from drifting
out of spec, leading to incompatabilities and hard-to-find bugs.

## Organization ##

Currently, the `.stf` files are organized as follows:

```
client.stf       ClientPacket specification
enums.stf        Enums and bitflags
objects.stf      Game object (with bitmask lengths)
parser.stf       Client/server parser tree
server.stf       ServerPacket specification
structs.stf      Structs used by Client/ServerPacket
```

## Getting started ##

To use this specification as more than a textual reference, you need a
`.stf` compiler. Right now, the only existing compiler is
**Transwarp** (link coming soon).

Using Transwarp, you can generate HTML documentation, ascii reference
tables, programming language headers, or anything you might need. All
you need, is to make a template file, that uses this data structure

## Contributors ##

The protocol specification in this repository, is based of the
collaborative work of the
[protocol-docs](https://github.com/artemis-nerds/protocol-docs/)
project, spearheaded by [Robert
J. Walker](https://github.com/rjwut). The conversion into `.stf`
format was done by [Christian Iversen](https://github.com/chrivers).