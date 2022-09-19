# Simple c compilation example

Here it's easy to see how make works with one target with a prerequisite. The general format is

```Makefile
target: prerequisite_1 prerequisite_2 prerequisite_3 ...
	command
	command
	command
	...
```

_Generally_ the target should be the name of the file output by the steps taken by the commands.

Make works with the prerequisite files' timestamps. If any prerequisites (or files in the dependency tree) have a newer timestamp than something further up the in dependency tree, then everything in that section of the dependency tree is recompiled.
