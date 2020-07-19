# 234-plv8-ubuntu18.04

done with:

```
rsync -nvr --include="*/" --include="plv8*" --exclude="*" --prune-empty-dirs /usr .
```

```
#create extension plv8;
ERROR: could not load library "/usr/lib/postgresql/12/lib/plv8-2.3.13.so": libc++.so.1: cannot open shared object file: No such file or directory
```

FIX:
```
$ sudo apt-get install libc++-dev
```
