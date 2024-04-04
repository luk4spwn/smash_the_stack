Compilation:

``` shell
gcc -m32 -no-pie -fno-stack-protector -ggdb -mpreferred-stack-boundary=2 -z execstack -o smash smash.c
```

we use these GCC flags to disable the protections (we are left with only the RELRO)
