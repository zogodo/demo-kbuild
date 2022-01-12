# demo-kbuild

## Overview
This demo-project showing how-to use KConfig in own project.
Simple script show information for last logins. It can forward output to current console or to file. Show last info for all user or for current-only.

Need KConfig interpritier in system(for example, kconfig-frontends project).

## Before
Install kconfig-frontends
```bash
# apt-get install kconfig-frontends

yum install autoconf automake libtool
git clone git@github.com:movidius/kconfig-frontends.git
cd kconfig-frontends
./bootstrap
make &&  make install
```

## Using
First clone repo:
```bash
git@github.com:skif-web/demo-kbuild.git
```

Next run KConfig for configuring:
```bash
cd demo-kbuild
kconfig-mconf KConfig
```

Last step: run script to test:
```
./getLast.sh
```