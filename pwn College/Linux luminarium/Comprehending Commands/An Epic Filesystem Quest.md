# An Epic Filesystem Quest

## Procedure
first i started the challenge from `pwn.college` and went to the terminal.
i got to know about ls `-a,cat,cd` from the module questions.
then after alllll the medhods mentioned in the Code .then i got the flag and pasted in the website.

## Code
`hhacker@commands~an-epic-filesystem-quest:~$ ls
a
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
GIST  challenge  flag  lib32   media  opt   run   sys  var
bin   dev        home  lib64   mnt    proc  sbin  tmp
boot  etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cd /flag
ssh-entrypoint: cd: /flag: Not a directory
hacker@commands~an-epic-filesystem-quest:/$ cd flag
ssh-entrypoint: cd: flag: Not a directory
hacker@commands~an-epic-filesystem-quest:/$ cd /flag
ssh-entrypoint: cd: /flag: Not a directory
hacker@commands~an-epic-filesystem-quest:/$ cd tmp
hacker@commands~an-epic-filesystem-quest:/tmp$ ls
bin  hsperfdata_root  tmp.G9qthVCks5
hacker@commands~an-epic-filesystem-quest:/tmp$ cd ..
hacker@commands~an-epic-filesystem-quest:/$ cd run
hacker@commands~an-epic-filesystem-quest:/run$ ls
apache2                   lock    sendsigs.omit.d  utmp
challenge                 log     shm              workspace
current-system            mount   sudo
dojo                      mysqld  systemd
firefox-restart-required  screen  user
hacker@commands~an-epic-filesystem-quest:/run$ cd challenge
hacker@commands~an-epic-filesystem-quest:/run/challenge$ ls
bin
hacker@commands~an-epic-filesystem-quest:/run/challenge$ cd..
ssh-entrypoint: cd..: command not found
hacker@commands~an-epic-filesystem-quest:/run/challenge$ cd ..
hacker@commands~an-epic-filesystem-quest:/run$ ls
apache2                   lock    sendsigs.omit.d  utmp
challenge                 log     shm              workspace
current-system            mount   sudo
dojo                      mysqld  systemd
firefox-restart-required  screen  user
hacker@commands~an-epic-filesystem-quest:/run$ cd ..
hacker@commands~an-epic-filesystem-quest:/$ ls
GIST  challenge  flag  lib32   media  opt   run   sys  var
bin   dev        home  lib64   mnt    proc  sbin  tmp
boot  etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
GIST  challenge  flag  lib32   media  opt   run   sys  var
bin   dev        home  lib64   mnt    proc  sbin  tmp
boot  etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.           GIST  challenge  flag  lib32   media  opt   run   sys  var
..          bin   dev        home  lib64   mnt    proc  sbin  tmp
.dockerenv  boot  etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cat /GIST
Lucky listing!
The next clue is in: /usr/share/racket/pkgs/scribble-lib/scribble/book

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/racket/pkgs/scribble-lib/scribble/book
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/book$ ls -a
.  ..  MESSAGE  compiled  lang  lang.rkt  style.tex
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/book$ cat MESSAGE
Tubular find!
The next clue is in: /opt/ghidra/Ghidra/Features/GhidraServer/data/yajsw-stable-13.09/lib/core/commons

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/book$ cd /opt/ghidra/Ghidra/Features/GhidraServer/data/yajsw-stable-13.09/lib/core/commons
hacker@commands~an-epic-filesystem-quest:/opt/ghidra/Ghidra/Features/GhidraServer/data/yajsw-stable-13.09/lib/core/commons$ ls -a
.                                 commons-io-2.11.0.jar
..                                commons-lang-2.6.jar
.NOTE                             commons-lang3-3.12.0.jar
commons-cli-1.5.0.jar             commons-logging-1.2.jar
commons-collections-3.2.2.jar     commons-text-1.10.0.jar
commons-configuration2-2.8.0.jar  commons-vfs2-2.9.0.jar
hacker@commands~an-epic-filesystem-quest:/opt/ghidra/Ghidra/Features/GhidraServer/data/yajsw-stable-13.09/lib/core/commons$ cat .NOTE
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/Documentation/networking/device_drivers/intel

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/ghidra/Ghidra/Features/GhidraServer/data/yajsw-stable-13.09/lib/core/commons$ cd /opt/linux/linux-5.4/Documentation/networking/device_drivers/intel
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/networking/device_drivers/intel$ ls -a
.        e100.rst    fm10k.rst  ice.rst    ipw2100.txt  ixgbe.rst
..       e1000.rst   i40e.rst   igb.rst    ipw2200.txt  ixgbevf.rst
INSIGHT  e1000e.rst  iavf.rst   igbvf.rst  ixgb.rst
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/networking/device_drivers/intel$ cat INSIGHT
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Operators
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/networking/device_drivers/intel$ cd /usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Operators
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Operators$ ls -a
.  ..  BLUEPRINT  Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Operators$ cat BLUEPRINT
Tubular find!
The next clue is in: /opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Operators$ cd /opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls -a
.  ..  NUGGET  libqmlwavefrontmeshplugin.so  plugins.qmltypes  qmldir
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cd NUGGET
ssh-entrypoint: cd: NUGGET: Not a directory
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls -a
.  ..  NUGGET  libqmlwavefrontmeshplugin.so  plugins.qmltypes  qmldir
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cat NUGGET
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls -a
.  ..  NUGGET  libqmlwavefrontmeshplugin.so  plugins.qmltypes  qmldir
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cat /opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh/NUGGET
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls -o
total 36
-rw-r--r-- 1 hacker   256 Oct  3 13:15 NUGGET
-rwxr-xr-x 1   1001 23192 Sep  6 00:21 libqmlwavefrontmeshplugin.so
-rw-r--r-- 1   1001  2428 Sep  6 00:21 plugins.qmltypes
-rw-r--r-- 1   1001   243 Sep  6 00:21 qmldir
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls-a
ssh-entrypoint: ls-a: command not found
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls -a
.  ..  NUGGET  libqmlwavefrontmeshplugin.so  plugins.qmltypes  qmldir
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls /opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh
NUGGET  libqmlwavefrontmeshplugin.so  plugins.qmltypes  qmldir
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard
CLUE-TRAPPED  _config.py      _importhook.py     _transformer.py
__init__.py   _decorators.py  _memo.py           _union_transformer.py
__pycache__   _exceptions.py  _pytest_plugin.py  _utils.py
_checkers.py  _functions.py   _suppression.py    py.typed
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cat /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard/CLUE_TRAPPED
cat: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard/CLUE_TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard
CLUE-TRAPPED  _config.py      _importhook.py     _transformer.py
__init__.py   _decorators.py  _memo.py           _union_transformer.py
__pycache__   _exceptions.py  _pytest_plugin.py  _utils.py
_checkers.py  _functions.py   _suppression.py    py.typed
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cat /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard/CLUE_TRAPPED
cat: /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard/CLUE_TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cat /usr/local/lib/python3.8/dist-packages/setuptools/_vendor/typeguard/CLUE-TRAPPED
Lucky listing!
The next clue is in: /usr/share/racket/pkgs/eopl/lang/compiled

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ ls /usr/share/racket/pkgs/eopl/lang/compiled
reader_rkt.dep  reader_rkt.zo
hacker@commands~an-epic-filesystem-quest:/opt/angr-management/_internal/PySide6/Qt/qml/Qt/labs/wavefrontmesh$ cd /usr/share/racket/pkgs/eopl/lang/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/eopl/lang/compiled$ ls -a
.  ..  .SPOILER  reader_rkt.dep  reader_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/eopl/lang/compiled$ cat .SPOILER
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/drivers/net/ethernet/amd/xgbe

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/eopl/lang/compiled$ ls /opt/linux/linux-5.4/drivers/net/ethernet/amd/xgbe
BRIEF-TRAPPED  xgbe-debugfs.c  xgbe-ethtool.c  xgbe-pci.c       xgbe-ptp.c
Makefile       xgbe-desc.c     xgbe-i2c.c      xgbe-phy-v1.c    xgbe.h
xgbe-common.h  xgbe-dev.c      xgbe-main.c     xgbe-phy-v2.c
xgbe-dcb.c     xgbe-drv.c      xgbe-mdio.c     xgbe-platform.c
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/eopl/lang/compiled$ ls /opt/linux/linux-5.4/drivers/net/ethernet/amd/xgbe/BRIEF-TRAPPED
/opt/linux/linux-5.4/drivers/net/ethernet/amd/xgbe/BRIEF-TRAPPED
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/eopl/lang/compiled$ ls /opt/linux/linux-5.4/drivers/net/ethernet/amd/xgbe
BRIEF-TRAPPED  xgbe-debugfs.c  xgbe-ethtool.c  xgbe-pci.c       xgbe-ptp.c
Makefile       xgbe-desc.c     xgbe-i2c.c      xgbe-phy-v1.c    xgbe.h
xgbe-common.h  xgbe-dev.c      xgbe-main.c     xgbe-phy-v2.c
xgbe-dcb.c     xgbe-drv.c      xgbe-mdio.c     xgbe-platform.c
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/eopl/lang/compiled$ cat /opt/linux/linux-5.4/drivers/net/ethernet/amd/xgbe/BRIEF-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{krrCwTeH1DkG-hpY_3HIpfA7srx.dljM4QDL5EjN0czW}`

## Reference
my ERRORS
