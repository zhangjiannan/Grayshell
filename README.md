Grayshell
=========

Some basic shell code, when I learn &lt;Gray Hat Hacking>


#How to run 

##Example1 : Buffer_overflow
//notice we start out at user privileges "$"

```
gcc overflow.c -ggdb -mpreferred-stack-boundary=2 -fno-stack-protector -o overflow
``` 

```
$gdb -g overflow 
(gdb) run
(gdb) info req eip
(gdb) q
```

##Example2 : Meet.c
//notice we start out at user privileges "$"

```
gcc meet.c -ggdb -mpreferred-stack-boundary=2 -fno-stack-protector -z execstack -o meet
``` 

```
$gdb -g overflow 
(gdb) run
(gdb) info req eip
(gdb) q
```
