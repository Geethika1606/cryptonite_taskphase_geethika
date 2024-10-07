# An Epic File Quest
Connected to the server and changed directory using cd command. Then used ls to read the current directory. Used cat with SECRET to read it as it was synonymous to HINT/CLUE and got a clue within it to proceed
further. Again changed directory according to the clue given, used ls to read it and cat to find the next clue. Follow the instructions given and repeated the process till flag was invoked.
***
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
SECRET  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin     challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat SECRET
Tubular find!
The next clue is in: /usr/share/icons/Humanity/actions

The next clue is *delayed* --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/icons/Humanity/actions
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/actions$ ls
128  16  22  24  32  48  64  DOSSIER  symbolic
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/actions$ ls -a
.  ..  128  16  22  24  32  48  64  DOSSIER  symbolic
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/actions$ cat DOSSIER
Yahaha, you found me!
The next clue is in: /usr/lib/python3.8/config-3.8-x86_64-linux-gnu
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/actions$ cd /usr/lib/python3.8/config-3.8-x86_64-linux-gnu
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3.8/config-3.8-x86_64-linux-gnu$ ls -a
.   CUE       Setup        config.c     install-sh          libpython3.8.a   makesetup         python.o
..  Makefile  Setup.local  config.c.in  libpython3.8-pic.a  libpython3.8.so  python-config.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3.8/config-3.8-x86_64-linux-gnu$ cat CUE
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/sympy/codegen

The next clue is *delayed* --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3.8/config-3.8-x86_64-linux-gnu$ cd /usr/local/lib/python3.8/dist-packages/sympy/codegen
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ ls -a
.         _init_.py        algorithms.py      cfunctions.py  cxxnodes.py  matrix_nodes.py  pyutils.py      tests
..        _pycache_        approximations.py  cnodes.py      fnodes.py    numpy_nodes.py   rewriting.py
EVIDENCE  abstract_nodes.py  ast.py             cutils.py      futils.py    pynodes.py       scipy_nodes.py
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cat EVIDENCE
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/tools/perf/arch/nds32/util

Watch out! The next clue is *trapped*. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cat /opt/linux/linux-5.4/tools/perf/arch/nds32/util
cat: /opt/linux/linux-5.4/tools/perf/arch/nds32/util: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ ls -a /opt/linux/linux-5.4/tools/perf/arch/nds32/util
.  ..  Build  DISPATCH-TRAPPED  header.c
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cat DISPATCH-TRAPPED
cat: DISPATCH-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cat DISPATCH
cat: DISPATCH: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cat DISPATCH-TRAPPED
cat: DISPATCH-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cat /opt/linux/linux-5.4/tools/perf/arch/nds32/util/DISPATCH-TRAPPED
Tubular find!
The next clue is in: /opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa

The next clue is *hidden* --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/codegen$ cd /opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa$ ls -a
.          fixed-multiply   int-max-min   pack                        test_msa_run_32r5el.sh
..         float-max-min    int-modulo    shift                       test_msa_run_64r6eb.sh
.TRACE     int-add          int-multiply  test_msa_compile_32r5eb.sh  test_msa_run_64r6el.sh
README     int-average      int-subtract  test_msa_compile_32r5el.sh
bit-count  int-compare      interleave    test_msa_compile_64r6eb.sh
bit-move   int-divide       logic         test_msa_compile_64r6el.sh
bit-set    int-dot-product  move          test_msa_run_32r5eb.sh
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa$ cat .TRACE
Lucky listing!
The next clue is in: /usr/local/BurpSuiteCommunity/jre/include

Watch out! The next clue is *trapped*. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa$ cat /usr/local/BurpSuiteCommunity/jre/include
cat: /usr/local/BurpSuiteCommunity/jre/include: Is a directory
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa$ ls -a /usr/local/BurpSuiteCommunity/jre/include
.  ..  SNIPPET-TRAPPED  classfile_constants.h  jawt.h  jni.h  jvmti.h  jvmticmlr.h  linux
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa$ cat /usr/local/BurpSuiteCommunity/jre/include/SNIPPET-TRAPPED
Great sleuthing!
The next clue is in: /opt/aflplusplus/qemu_mode/qemuafl/contrib/ivshmem-client

The next clue is *hidden* --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/QEMU-Nyx/tests/tcg/mips/user/ase/msa$ cd /opt/aflplusplus/qemu_mode/qemuafl/contrib/ivshmem-client
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/contrib/ivshmem-client$ ls -a
.  ..  .LEAD  ivshmem-client.c  ivshmem-client.h  main.c  meson.build
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/contrib/ivshmem-client$ cat .LEAD
Lucky listing!
The next clue is in: /opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/.fingerprint/indexmap-6f6526087fd2d7aa

The next clue is *hidden* --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/contrib/ivshmem-client$ cd /opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/.fingerprint/indexmap-6f6526087fd2d7aa
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/.fingerprint/indexmap-6f6526087fd2d7aa$ ls -a
.  ..  .README  run-build-script-build-script-build  run-build-script-build-script-build.json
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/.fingerprint/indexmap-6f6526087fd2d7aa$ cat .README
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{0k5CxyO5Jp-uJLPUy-TNIohHdds.dljM4QDLykjN0czW}
***
Resources used:Dojo
