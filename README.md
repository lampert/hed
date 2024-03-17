# Command line hex editor

```
HED hex editor help
p#       Set byte position (0x for hex)
r#       Position to record number. If # is blank, align on current rec
$        Set position to last record
.        Show current record
#        Forward # records
<enter>  Forward 1 record
-#       Backward # records
l#       Set logical record length (default 256)
editing
    e OFFSET       interactive edit mode, byte by byte. ^d to stop
    e OFFSET HEX   at OFFSET, set HEX bytes;    e 0x1234 FF EE
    e OFFSET "string"  at OFFSET, set string;   e 1000 "Hello"
    OFFSET: ...    : indicates edit at offset;  0x999: "Hello" 00
w        Write changes
?        Status, shoow pending edits
q or x   Exit
```
