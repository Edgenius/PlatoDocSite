+++
prev = "/editor/"
next = "/editor/options/"
toc = true
date = "2017-01-03T11:27:55+11:00"
title = "Single line text"
weight = 5

+++

### Format
{{% notice note  %}}
<a name="HM-EDITOR-010" class="anchor"></a>
It splits the text input into pieces with our format syntax, for example, date format YYYY/MM/DD. 
{{% /notice  %}}

h4. Sample format
Placeholder character is always #, separate can be any characters except #.
```
##:##:##
##/##/##
(##) (###) (#########)
```

You can define the various length, by [m-n] format, or `*` to indicate any length.
```
#[0-3]:##:#*
```

h4. Number format
Placeholder is `n`.

```
dd:dd:dd
##:dd:##
```

h4. Date and Time format

Date YYYY/MM/DD
Time hh:mm:ss

Please note, these letter are case sensitive. yyyy/mm/dd won't render correctly.

[moment.js](http://momentjs.com/docs/)

h4. Reserved characters and escape
```
#                        -> character placeholder
n                        -> digit placeholder
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
