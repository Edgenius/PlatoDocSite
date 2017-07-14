+++
title = "Text Field with Format Rule"
weight = 5
+++

{{% notice tip  %}}
<a name="HM-EDITOR-010" class="anchor"></a>
With format property, you can split Text Field into a few of pieces. For example, you can set YYYY/MM/DD for a Date type field.
{{% /notice %}}

In `Signle Line Text` properties popup, there is a "Format" property. Only if the text type is `Single Line Text, Date, Time or Date and Time`, you can use below rules to set up the format rule to make fine control on this field.

![Text Field Format](/images/page/form/text-type.png)

As the example, on below screenshot, it is set to `Date` type and has `YYYY-MM-DD` as format rule. So you can see this text field are splitted into 3 smaller input fields to restrict only `YYYY-MM-DD` format date can be inputted.

![Text Field Format](/images/page/form/text-format.png)

The format rule can be categoried into 2 kinds. One is for `Text` field, the other is for `Date and Time` field. 

#### Format for Text field 

Placeholder character can be `#`(character) or `d`(digit).  


In below example, the first format rule will split the field into 3 parts, with separator `:`.  The second example is also 3 splitted parts with `/` as separator. The third format rule is a good example for telephone number input.

```
##:##:##
##/##/##
(##) (###) (#########)
```

Below examples include the digit only or digit and text mixed. Their separator is `:`. 

```
dd:dd:dd
##:dd:##
```

Generally, the input is fixed length. For example, `###:##` will be 3 characters in first part and 2 character in second part. You can define length by [m-n] format, or `*` to indicate any length. For example, below 3 parts input,  the first part can be 0 to 3 characters, then 2 characters in the second part, and any of length of characters in last part.
```
#[0-3]:##:#*
```

**Reserved characters and escape**

```
#                        -> character placeholder
d                        -> digit placeholder
[], digit 0 to 9, - or * -> length definition
\                        -> escape 
```

If the separator is reserved character, you can escape it by `\`.  For example, `##\###\###:##` format rule, its separator is `#` which is escaped by `\`. So input `xx#yy#cc` is valid input.

More examples:
```
-> Separator is [,  ] and *
##\[##\]##\*##  > xx[yy]cc*dd

-> If spearator is '\', it must escape itself in format '\\'
##\\##\\##  > xx\yy\cc  

```

#### Format for Date and Time field 

Date `YYYY/MM/DD`

Time `hh:mm:ss`

Please note, these letter are case sensitive. yyyy/mm/dd won't render correctly.

For more format details, please check out [moment.js date time format](http://momentjs.com/docs/)

