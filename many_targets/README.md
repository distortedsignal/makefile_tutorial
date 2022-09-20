# The Make tree
This is a good example of how Make tracks timestamps through the tree.

The `blah.c` target makes a file. The `blah.o` target compiles the previously created c file. The `blah` target makes a `blah` file. To force make to create and recompile the file, `rm blah.c`. To force a recompilation of `blah`, `touch blah.c` updating its timestamp.