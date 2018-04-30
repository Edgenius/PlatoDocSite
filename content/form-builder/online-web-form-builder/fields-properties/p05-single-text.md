+++
title = "TEXT FIELD PROPERTIES"
weight = 305
description = "Customise your text fields with PlatoForms Text Field Properties."
+++

Use this section to learn how to customise your text fields.

## Text Type

In the *Text Input* field's properties panel, you can specify the type of text your users can input. To switch the text type, use the *toggle switch* in the top left. 

There are seven text types:

* Single Line Text
* Multiple Lines Text
* Numbers
* Email
* URL
* Date
* Time
* Date and Time

![text-field-properties](/images/text-field-properties.png)

## Format Rule

{{% notice tip  %}}
<a name="HM-EDITOR-010" class="anchor"></a>
Use the format property to split a Text Field into two or more parts. This works great for adding the year, month and day (YYYY/MM/DD) to a date field.
{{% /notice %}}


The format property allows you to **split the text field into multiple parts**. This is helpful when formatting for numerical calendar dates; for example, if you entered YYYY/MM/DD, the field would divide into three sections to allow for the year, month, and day.

The format rule is available for *Single Line Text*, *Date*, *Time*, and *Date and Time*.

In the below example, you can see the text type is *Date*, and it has the format rule applied; YYYY-MM-DD. In the form preview, you can see that three small input boxes are available for each division of the format rule.

![format-rule](/images/format-rule.png)

### Formatting a Text Field

Compatible placeholder characters for the format field are:

`#` : For **characters** 

`d` : For **digits**

You can signal a divide in the field using a separator. Some examples of these are:

* **Colon**
  `##:##:##` 
  Suggested use: **time**.
* **Slash**
  `##/##/##` 
  Suggested use: **date**.
* **Parenthesis**
  `(dd) (ddd) (ddddddddd)` 
  Suggested use: **telephone number**.

Hint: You can mix `#` (characters) and `d` (digits) if your field needs it; for example, `##/dd/##`.


#### Customising the Length of the Field

- **Fixed length**
  The number of characters or digits is determined by the amount of `#` or `d`.
  *Example:*
  `##/###` = **Part 1:** three characters | **Part 2:** two characters


- **Variable length**
  You can **set a length range** by using `[m-n]` format, or use `*` to indicate any length. 
  *Example*
  `#[0-3]:##:#*` = **Part 1:** three characters | **Part 2:** zero to three characters | **Part 3:** any number of characters.



#### **Reserved Characters and Escape**

If the separator you want to use is a reserved character, you can `escape` (force it) it by using `\` one place before the divide.

Here are some examples of using `\` to separate fields:

- `##\###\###`
  The separator is `#`. Use `\` to force the break; place it one character before the split. The render looks like `xx#yy#cc`.


- `##\[##\]##\*##
  The separator is `[, ]`, and `*`. The render looks like `xx[yy]cc*dd`.


- `##\\##\\##`
  The separator is `\`. The render looks like `##\##\##`.



#### Formatting the Date and Time Field

- **Date** 
  `YYYY/MM/DD`
- **Time**
   `hh:mm:ss`

***Please Note:*** The letters **are case-sensitive**, therefore, `yyyy/mm/dd` (lowercase) won’t render correctly.

We use [moment.js](https://momentjs.com/) to convert date and time format rule. Learn more about [formatting date and time with moment.js](http://momentjs.com/docs/).



#### Separator in PDF

In the *format* rules (of the field property), you can change the separators rendering settings for PDF. If the separator is natively a part of the PDF, then select the option *No* for *Print separator in PDF*. This stops duplicate separators being generated when the PDF is rendered.



![print-sep](/images/print-sep.png)















