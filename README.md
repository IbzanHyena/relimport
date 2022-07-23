# relimport

Defines a simple monad to import a script from a relative path.

## Example

```
relimport 'localfile'
relimport '../file.ijs'
relimport 'subdir/file.ijs'
```

## Installation

Clone this repo into a location of your chosing.
Then, open the file `j903/system/main/stdlib.ijs` and add a line that loads this script.
Change the filepath as required.

```
NB. etc.
load=: 3 : 0 NB. omitted
loadd=: 1&load
require=: 3 : 0 NB. omitted
NB. ---- Patched in ----
require '~Projects/relimport/relimport.ijs'
NB. ---- Patched in end ----
scripts=: scripts_j_
NB. etc.
```

Alternatively, add the contents of `relimport.ijs` to `stdlib.ijs`
