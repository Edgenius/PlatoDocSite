+++
prev = "/prev/path"
next = "/next/path"
toc = true
date = "2017-01-03T11:27:55+11:00"
title = "single text"
weight = 5

+++



### Format
{{% notice note  %}}
<a name="HM-EDITOR-010" class="anchor"></a>
Format can separate input text with spearator,e.g, ##:##:##.  If separator is #, spearator can use *, i.e, **#**#**. 

Sample format, placeholder character is always #, separate can be any characters except #.
```
##:##:##
##/##/##
(##) (###) (#########)
```

You can define the various length, by [m-n] format, or `*` to indicate any length.
```
#[0-3]:##:#*
```

For number, you can use `d` as placeholder instead of `#`.

```
dd:dd:dd
##:dd:##
```

All reserved characters list here:
```
#                        -> character placeholder
d                        -> digit placeholder
[], digit 0 to 9, - or * -> length range
\                        -> escape 
```

If the spearator is reserved charater, you must escape it by `\`. 

```
##\###\###:##  -> xx#yy#cc


##\[##\]##\*##  > xx[yy]cc*dd

-> If spearator is '\', it must escape itself in format '\\'
##\\##\\##  > xx\yy\cc  

```

{{% /notice %}}
