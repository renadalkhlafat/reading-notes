# Regular Expression (regex)
A special sequence of characters that helps you match or find other strings or sets of strings, using a specialized syntax held in a pattern.
The Python module re provides full support for Perl-like regular expressions in Python

+  match function 
This function attempts to match RE pattern to string with optional flags.

`re.match(pattern, string, flags=0)`

+ search function
This function searches for first occurrence of RE pattern within string with optional flags.

`re.search(pattern, string, flags=0) `

+ Matching Versus Searching

**Example**:

```python


import re

line = "Cats are smarter than dogs";

matchObj = re.match( r'dogs', line, re.M|re.I)
if matchObj:
   print "match --> matchObj.group() : ", matchObj.group()
else:
   print "No match!!"

searchObj = re.search( r'dogs', line, re.M|re.I)
if searchObj:
   print "search --> searchObj.group() : ", searchObj.group()
else:
   print "Nothing found!!"
```

+ Search and Replace
One of the most important re methods that use regular expressions is sub.

`re.sub(pattern, repl, string, max=0)`

## shutil
module includes high-level file operations such as copying and archiving.

+ Copying Files `copyfile()`
+ Copying File Metadata `copystat().` , `copymode()`
+ copy a directory `copytree().`
+ Finding Files `which()`
+ Archives `get_archive_formats()` ,`make_archive() `,`get_unpack_formats().`

## Automation:
 A process in which a manually performed action is transformed into one that happens automatically.
 - Automating a task means that it can run a lot quicker, most of the time
 - Automating a task means there’s less potential for mistakes, as the impact of human error is mitigated.