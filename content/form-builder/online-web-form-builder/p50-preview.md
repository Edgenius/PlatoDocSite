+++
title = "Form Preview"
weight = 50
description = "Preview your form can check what it looks like on web page. It can test form submit and PDF generation."
+++

Clicking "Preview Form" button in the toolbar can open a new window to check what your form looks like. This form can be filled and submitted as same as the form you will share with the public.  Here introduce some tips that help you build and preview forms more efficiently.

![Text Preview Data](/images/page/form/preview.png)


#### Disable Form Validation
Normally, the form may run some validation at your submitting, for example, maximum or minimum length or numeric value required etc. This is good if you want to collect enough and valid data from your customers. However, this may be annoying when you preview the form. For example, if your web form has multiple steps or you want to preview PDF with some certain fields, you can turn off "Form Validation", so the form still can be submitted even it is invalid.


#### Fill Sample Data

In form builder, you can fill some data in preview section in its field properties popup. They can use both Form Preview or PDF Preview. For example, if you input "John Joe" into this text input field in its `preview section`. At web form preview page, click "Fill Preview Data" button in its top function bar, this input field will be automatically filled in "John Joe" as sample data. This can save lots of your time when you want to preview generated PDF after form submitted. In form builder page, "John Joe" is also rendered in PDF when you press `Preview PDF`.

Note, not all fields can set pre-filling data.  Only `SingleText`, `MultiText`, `Choice`, `Dropdown` and `Signature` can have sample data. For `File Upload` or `Captcha`, you always have to fill them in manually.

![Text Preview Data](/images/page/form-preview/text-preview.png)

#### Preview PDF after form submitted

Once you submit the form, you can check out the generated PDF by your form data. Simply press that "Preview PDF" button on its top functional bar.


#### Sample and Default Option

In `Choice` or `Dropdown` field, you can set the default selected value in the form. It means that choice is selected once the form is loaded. You must understand the sample selection and default selection are the different things. In below example, the above blue highlight area is the default value, the left below one is sample value.

![Text Preview Data](/images/page/form/sample-default-option.png)