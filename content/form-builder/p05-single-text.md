+++
title = "Text Field with Format Rule"
weight = 5
+++

{{% notice tip  %}}
<a name="HM-EDITOR-010" class="anchor"></a>
With format property, you can split Text Field into a few of parts. For example, you can set YYYY/MM/DD for a Date type field.
{{% /notice %}}

In `Signle Line Text` properties popup, there is a "Format" property. Only if the text type is `Single Line Text, Date, Time or Date and Time`, you can use below rules to set up the format to add fine control over this field.

![Single line text Type](/images/page/form/text-type.png)

As the example, on below screenshot, it is set to `Date` type and has `YYYY-MM-DD` as format rule. So you can see this text field are splitted into 3 smaller input fields to restrict only `YYYY-MM-DD` format date can be inputted.

![Text Field Format](/images/page/form/text-format.png)

The format rule can be categoried into 2 kinds. One is for `Text` field, the other is for `Date and Time` field. 

#### Format for Text field 

Placeholder character can be `#`(character) or `d`(digit).  


In below example, the first format rule will split the field into 3 parts with `:` as separator.  The second example is also 3 splitted parts with `/` as separator. The third format rule is a good example for telephone number input.

```
##:##:##
##/##/##
(##) (###) (#########)
```

Format rules `dd:dd:dd` is  the digit only with separator  `:`. 

Format rules `##:dd:##` is the digit and text mixed with separator  `:`. 


Generally, the input is fixed length. For example, `###:##` will be 3 characters in its first part and 2 character in its second part. You can define length range by `[m-n]` format, or `*` to indicate any length. For example, this format rule `#[0-3]:##:#*` is 3 parts,  the first part can be 0 to 3 characters, then 2 characters in the second part, and any of length of characters in last part.

**Reserved characters and escape**

```
#                        -> character placeholder
d                        -> digit placeholder
[], digit 0 to 9, - or * -> length definition
\                        -> escape 
```

If the separator is a reserved character, you can escape it by `\`.  

Some examples: 

Format rule `##\###\###:##`, its separator is `#` which is escaped by `\`. Its render looks like `xx#yy#cc`.

Format rule `##\[##\]##\*##`, its separator is `[`,  `]` and `*` and its render looks like `xx[yy]cc*dd`. 

Format rule `##\\##\\##`, its spearator is `\` which is escaped by its leading `\`.


#### Format for Date and Time field 

Date `YYYY/MM/DD`

Time `hh:mm:ss`

Please note, these letter are case sensitive. yyyy/mm/dd won't render correctly.

We use `moment.js` to convert date and time format rule. so if you want to more flexible date and time format, check out [the date and time format paragraph in its documentation](http://momentjs.com/docs/).


#### Separator in PDF
In format rule property, you can change its separator rendering mode in PDF. For example, if the separator `:` is already exist in your PDF, you can select `No` in `Print separator in PDF` in its pop menu. This separator `:` character won't render into PDF when PlatoForms generates it.

![Separator Print Option](/images/page/form/separator-print.png)