# Help for Builtins

## Procedure
i started the challenge, connected to terminal<br>
i used `help` and it gave me all the commands in terminal, then i saw challenge was a 
command, hence i used `help chellenge` and got to know about secret and how to get flag.
then typed `challenge --secret cyP0TreI` and got my flag.
Pasted the flag into the flag box.

## bash
`Connected!
hacker@man~help-for-builtins:~$ help
GNU bash, version 5.2.32(1)-release (x86_64-pc-linux-gnu)
These shell commands are defined internally.  Type `help' to see this list.
Type `help name' to find out more about the function `name'.
Use `info bash' to find out more about the shell in general.
Use `man -k' or `info' to find out more about commands not in this list.

A star (*) next to a name means that the command is disabled.

 job_spec [&]                          history [-c] [-d offset] [n] or hi>
 (( expression ))                      if COMMANDS; then COMMANDS; [ elif>
 . filename [arguments]                jobs [-lnprs] [jobspec ...] or job>
 :                                     kill [-s sigspec | -n signum | -si>
 [ arg... ]                            let arg [arg ...]
 [[ expression ]]                      local [option] name[=value] ...
 alias [-p] [name[=value] ... ]        logout [n]
 bg [job_spec ...]                     mapfile [-d delim] [-n count] [-O >
 bind [-lpsvPSVX] [-m keymap] [-f fi>  popd [-n] [+N | -N]
 break [n]                             printf [-v var] format [arguments]
 builtin [shell-builtin [arg ...]]     pushd [-n] [+N | -N | dir]
 caller [expr]                         pwd [-LP]
 case WORD in [PATTERN [| PATTERN]..>  read [-ers] [-a array] [-d delim] >
 cd [-L|[-P [-e]] [-@]] [dir]          readarray [-d delim] [-n count] [->
 challenge [--fortune] [--version] [>  readonly [-aAf] [name[=value] ...]>
 command [-pVv] command [arg ...]      return [n]
 compgen [-abcdefgjksuv] [-o option]>  select NAME [in WORDS ... ;] do CO>
 complete [-abcdefgjksuv] [-pr] [-DE>  set [-abefhkmnptuvxBCEHPT] [-o opt>
 compopt [-o|+o option] [-DEI] [name>  shift [n]
 continue [n]                          shopt [-pqsu] [-o] [optname ...]
 coproc [NAME] command [redirections>  source filename [arguments]
 declare [-aAfFgiIlnrtux] [name[=val>  suspend [-f]
 dirs [-clpv] [+N] [-N]                test [expr]
 disown [-h] [-ar] [jobspec ... | pi>  time [-p] pipeline
 echo [-neE] [arg ...]                 times
 enable [-a] [-dnps] [-f filename] [>  trap [-lp] [[arg] signal_spec ...]
 eval [arg ...]                        true
 exec [-cl] [-a name] [command [argu>  type [-afptP] name [name ...]
 exit [n]                              typeset [-aAfFgiIlnrtux] name[=val>
 export [-fn] [name[=value] ...] or >  ulimit [-SHabcdefiklmnpqrstuvxPRT]>
 false                                 umask [-p] [-S] [mode]
 fc [-e ename] [-lnr] [first] [last]>  unalias [-a] name [name ...]
 fg [job_spec]                         unset [-f] [-v] [-n] [name ...]
 for NAME [in WORDS ... ] ; do COMMA>  until COMMANDS; do COMMANDS-2; do>
 for (( exp1; exp2; exp3 )); do COMM>  variables - Names and meanings of >
 function name { COMMANDS ; } or nam>  wait [-fn] [-p var] [id ...]
 getopts optstring name [arg ...]      while COMMANDS; do COMMANDS-2; do>
 hash [-lr] [-p pathname] [-dt] [nam>  { COMMANDS ; }
 help [-dms] [pattern ...]
hacker@man~help-for-builtins:~$ challenge help
Incorrect usage! Please read the help page for the challenge builtin!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "cyP0TreI".
hacker@man~help-for-builtins:~$ challenge --secret cyP0TreI
Correct! Here is your flag!
pwn.college{cyP0TreIH05JPMi4c1_hE4dIWEN.dRTM5QDLyIDO0czW}`

## Reference
Didnt use
