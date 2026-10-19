Zotero
======
A lazy work in progress tentative to port Zotero to NetBSD

Current status: it seems to work using GNU coreutils to build. These are the preresiquites steps to run out of my memory... so probably I forgot something 

As root

```
pkgin install firefox153 python3.13
pkgin install coreutils findutils gsed grep gtar gawk gmake bash diffutils
pkgin install nodejs
```

From the project root folder:

```
mkdir -p ~/bin/
ln -s /usr/pkg/bin/python3.13 ~/bin/python
ln -s /usr/pkg/bin/bash /bin/bash
export PATH=/usr/pkg/gnu/bin:$PATH
./app/scripts/build_and_run -f
```

Original README
======
[![CI](https://github.com/zotero/zotero/actions/workflows/ci.yml/badge.svg)](https://github.com/zotero/zotero/actions/workflows/ci.yml)

[Zotero](https://www.zotero.org/) is a free, easy-to-use tool to help you collect, organize, cite, and share your research sources.

Please post feature requests or bug reports to the [Zotero Forums](https://forums.zotero.org/). If you're having trouble with Zotero, see [Getting Help](https://www.zotero.org/support/getting_help).

For more information on how to use this source code, see the [Zotero documentation](https://www.zotero.org/support/dev/source_code).
