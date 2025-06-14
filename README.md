Breakit!
---

Tool to collect, write, and generate `PKGBREAK` (AOSCnese for `Breaks:`)
information from a package tree (such as
[aosc-os-abbs](https://github.com/AOSC-Dev/aosc-os-abbs)).

Usage
---

To build:

```
cargo build --release
```

To use:

```
Usage: breakit [OPTIONS] [PACKAGES]...

Arguments:
  [PACKAGES]...
          Package name

Options:
  -C <TREE>
          Path of ABBS tree
          
          [env: ABBS_TREE=]

  -t, --type <KIND>
          Breakage kind

  -w, --write
          Write PKGBREAK

      --write-group <WRITE_GROUP>
          Write rebuild group file

      --bump-rel
          Bump REL for broken packages.
          
          Packages that are already updated in the topic will not be bumped (in comparsion with local stable branch).

  -h, --help
          Print help (see a summary with '-h')

  -V, --version
          Print version
```
