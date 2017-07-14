+++
title = "Text input with Format Rule"
weight = 5
+++

{{% notice tip  %}}
<a name="HM-EDITOR-010" class="anchor"></a>
With format rule, you can split Text Field into a few of pieces. For example, you can set YYYY/MM/DD for a date type field.
{{% /notice %}}

In text field property popup, there is a "format" value. If the text field is `Single Line Text`, `Date`, `Time` or `Date and Time`, you can use below rules to set up the format.

![Text Field Format](/images/page/form/text-type.png)


As the example, in this is screenshot, it is Date type. It sets the date format to `YYYY-MM-DD`, so you can see the form fields are split into 3 smaller input fields to allow user input correct `YYYY-MM-DD` format date.

![Text Field Format](/images/page/form/text-format.png)


#### Format for Single Line Text input


Placeholder character can be `#`(character) or `d`(digit).  


In below example, the first format rule will split the fields into 3 parts, with separator `:`.  The second example is also 3 input fields, but with `/` as separator. The third format rule is good example for telephone number input.

```
##:##:##
##/##/##
(##) (###) (#########)
```

Below examples includes the digit or mixed digit and text in format rule:

```
dd:dd:dd
##:dd:##
```

Generally, it is fixed length input. For example, same length with the length of placeholder characters. You can define length by [m-n] format, or `*` to indicate any length.


In this example, it will be split into 3 fields. The first  input can be 0 to 3 characters, then 2 characters, and the any length of characters.
```
#[0-3]:##:#*
```

#### Reserved characters and escape

```
#                        -> character placeholder
n                        -> digit placeholder
[], digit 0 to 9, - or * -> length range
\                        -> escape 
```

If the separator is reserved character, you can escape it by `\`. 

```
##\###\###:##  -> xx#yy#cc


##\[##\]##\*##  > xx[yy]cc*dd

-> If spearator is '\', it must escape itself in format '\\'
##\\##\\##  > xx\yy\cc  

```


#### Format for Date and Time input

Date `YYYY/MM/DD`

Time `hh:mm:ss`

Please note, these letter are case sensitive. yyyy/mm/dd won't render correctly.

For more format details, please check out [moment.js date time format](http://momentjs.com/docs/)

