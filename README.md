# German Dictionary for Eclipse

This adds a German dictionary to the spelling engine from [Eclipse JDT](https://www.eclipse.org/jdt/). It is based on the dictionary [igerman98](https://www.j3e.de/ispell/igerman98/) (Version: 20161207) from Björn Jacke.


## Requirements

  * Eclipse 2018-09 or newer


## Installation

  * Open  _Help > Install New Software_  and add a new repository with location [https://oleosterhagen.github.io/update-site/](https://oleosterhagen.github.io/update-site/)
  * Install  _Germany Dictionary_  from this site.
  * Enable spell checking in  _Window > Preferences: General > Editors > Text Editors > Spelling_
  * Choose Platform Dictionary: Deutsch (Deutschland)
  * :warning: Ensure encoding is set to UTF-8 (on Linux, Mac) or CP1252 (on Windows).


## Limitations

  * The encoding is not stored in the dictionary ([Eclipse Bug 262025](https://bugs.eclipse.org/bugs/show_bug.cgi?id=262025)) and must therefore be set correctly (see above). To minimize problems this dictionary is distributed as two OS specific plug-ins, one with encoding UTF-8 (Linux, Mac) and another with encoding CP1252 (Windows).
  * The spelling engine from Eclipse JDT uses a simple word list without a separate affix file. For German this results in a very large file with 364.814 words which must be kept in memory.
