# An Epic Filesystem Quest

## Procedure
i started the challenge and then connected my terminal. <br>
I used `ls -a` and then used `cd` and used `cat` to find all the clues and then at the 
end found the flag.

## bash
`Connected!
hacker@commands~an-epic-filesystem-quest:~$ pwd
/home/hacker
hacker@commands~an-epic-filesystem-quest:~$ cd ../
hacker@commands~an-epic-filesystem-quest:/home$ cd ..
hacker@commands~an-epic-filesystem-quest:/$ ls
TEASER  challenge  flag  lib32   media  opt   run   sys  var
bin     dev        home  lib64   mnt    proc  sbin  tmp
boot    etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.           TEASER  challenge  flag  lib32   media  opt   run   sys  var
..          bin     dev        home  lib64   mnt    proc  sbin  tmp
.dockerenv  boot    etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cd flag
ssh-entrypoint: cd: flag: Not a directory
hacker@commands~an-epic-filesystem-quest:/$ cd challenge
hacker@commands~an-epic-filesystem-quest:/challenge$ ls
DESCRIPTION.md
hacker@commands~an-epic-filesystem-quest:/challenge$ cd ..
hacker@commands~an-epic-filesystem-quest:/$ cd home
hacker@commands~an-epic-filesystem-quest:/home$ ls
hacker
hacker@commands~an-epic-filesystem-quest:/home$ cd hacker
hacker@commands~an-epic-filesystem-quest:~$ ls
a
hacker@commands~an-epic-filesystem-quest:~$ cd a
ssh-entrypoint: cd: a: Not a directory
hacker@commands~an-epic-filesystem-quest:~$ cat a
pwn.college{Ebr8oWXy5ba4r_v_HXYhbrLkRX2.dNzM4QDLyIDO0czW}
hacker@commands~an-epic-filesystem-quest:~$ cd ../
hacker@commands~an-epic-filesystem-quest:/home$ cd ../
hacker@commands~an-epic-filesystem-quest:/$ cd ..
hacker@commands~an-epic-filesystem-quest:/$ cd TEASER
ssh-entrypoint: cd: TEASER: Not a directory
hacker@commands~an-epic-filesystem-quest:/$ cat TEASER
Great sleuthing!
The next clue is in: /usr/lib/python3/dist-packages/setuptools_scm/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ pwd
/
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/setuptools_scm/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/setuptools_scm/__pycache__$ ls -a
.                               file_finder_hg.cpython-38.pyc
..                              git.cpython-38.pyc
.CLUE                           hacks.cpython-38.pyc
__init__.cpython-38.pyc         hg.cpython-38.pyc
__main__.cpython-38.pyc         integration.cpython-38.pyc
config.cpython-38.pyc           utils.cpython-38.pyc
discover.cpython-38.pyc         version.cpython-38.pyc
file_finder.cpython-38.pyc      win_py31_compat.cpython-38.pyc
file_finder_git.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/setuptools_scm/__pycache__$ cat .CLUE
Tubular find!
The next clue is in: /opt/linux/linux-5.4/tools/arch/sparc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/setuptools_scm/__pycache__$ cd /opt/linux/linux-5.4/tools/arch/sparc
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/sparc$ ls -a
.  ..  SECRET  include
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/sparc$ cat SECRET
Lucky listing!
The next clue is in: /usr/share/racket/pkgs/redex-examples

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/tools/arch/sparc$ cd /usr/share/racket/pkgs/redex-examples
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ ls -a
.  ..  .TIP  LICENSE.txt  info.rkt  redex
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ cat .TIP
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/sympy/parsing/autolev

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ cat /usr/lib/python3/dist-packages/sympy/parsing/autolev
cat: /usr/lib/python3/dist-packages/sympy/parsing/autolev: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ ls /usr/lib/python3/dist-packages/sympy/parsing/autolev
Autolev.g4       __pycache__                 _parse_autolev_antlr.py
POINTER-TRAPPED  _antlr                      test-examples
__init__.py      _listener_autolev_antlr.py
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ /usr/lib/python3/dist-packages/sympy/parsing/autolev/POINTER-TRAPPED
ssh-entrypoint: /usr/lib/python3/dist-packages/sympy/parsing/autolev/POINTER-TRAPPED: Permission denied
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ cat /usr/lib/python3/dist-packages/sympy/parsing/autolev/POINTER-TRAPPED
Great sleuthing!
The next clue is in: /usr/lib/python3/dist-packages/_pytest/_code
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/redex-examples$ cd /usr/lib/python3/dist-packages/_pytest/_code
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_code$ ls
WHISPER  __init__.py  __pycache__  _py2traceback.py  code.py  source.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_code$ cat WHISPER
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/scribble-lib/scribble/lncs/compiled

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/_pytest/_code$ cd /usr/share/racket/pkgs/scribble-lib/scribble/lncs/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/lncs/compiled$ ls v-a
ls: cannot access 'v-a': No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/lncs/compiled$ ls -a
.  ..  .DISPATCH  lang_rkt.dep  lang_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/lncs/compiled$ cat .DISPATCH
Tubular find!
The next clue is in: /usr/share/racket/pkgs/srfi-lib/srfi/%3a13/compiled

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/scribble-lib/scribble/lncs/compiled$ cd /usr/share/racket/pkgs/srfi-lib/srfi/%3a13/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/srfi-lib/srfi/%3a13/compiled$ ls
LEAD  strings_rkt.dep  strings_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/srfi-lib/srfi/%3a13/compiled$ cat LEAD
Great sleuthing!
The next clue is in: /usr/lib/python3/dist-packages/sage/homology/__pycache__

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/srfi-lib/srfi/%3a13/compiled$ cd /usr/lib/python3/dist-packages/sage/homology/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sage/homology/__pycache__$ ls
SNIPPET
__init__.cpython-38.pyc
algebraic_topological_model.cpython-38.pyc
all.cpython-38.pyc
cell_complex.cpython-38.pyc
chain_complex.cpython-38.pyc
chain_complex_homspace.cpython-38.pyc
chain_complex_morphism.cpython-38.pyc
chain_homotopy.cpython-38.pyc
chains.cpython-38.pyc
cubical_complex.cpython-38.pyc
delta_complex.cpython-38.pyc
examples.cpython-38.pyc
hochschild_complex.cpython-38.pyc
homology_group.cpython-38.pyc
homology_morphism.cpython-38.pyc
homology_vector_space_with_basis.cpython-38.pyc
koszul_complex.cpython-38.pyc
matrix_utils.cpython-38.pyc
simplicial_complex.cpython-38.pyc
simplicial_complex_homset.cpython-38.pyc
simplicial_complex_morphism.cpython-38.pyc
simplicial_complexes_catalog.cpython-38.pyc
simplicial_set.cpython-38.pyc
simplicial_set_catalog.cpython-38.pyc
simplicial_set_constructions.cpython-38.pyc
simplicial_set_examples.cpython-38.pyc
simplicial_set_morphism.cpython-38.pyc
tests.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sage/homology/__pycache__$
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sage/homology/__pycache__$ cat SNIPPET
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{Y2xvBiOP7vqVJh27FfCHPpPPI_4.dljM4QDLyIDO0czW}`

## Reference
Didnt use
