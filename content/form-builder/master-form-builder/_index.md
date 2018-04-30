+++
title = "MASTER FORM BUILDER"
description = "With a master form you can link multiple different PDF forms. With PlatoForms creating a master form is simple."
weight = 8
+++

When building a master form, you don't need to upload a PDF beforehand. Click *Create Master For Multiple PDFs*, and you'll arrive at the *Form Builder*. On the form builder, there are three main sections:

* Form Widget Attributes
* Form Widget Preview
* Form Widget List



![master-build-layout](/images/master-build-layout.png)



## Step 1: Building Your Master Form

Get started building your form. 

### Adding Fields to Your Form

At the top left of the page is the *Toolbar*. Use the ***+ Add*** button to add various fields to your form. The options are categorised by compatibility; either *Form and PDF* or *Form Only*.

| Form and PDF | Form Only    |
| ------------ | ------------ |
| Text Input   | Page Divider |
| Choice       | Description  |
| Dropdown     | ReCaptcha    |
| Signature    | File Upload  |

### Arranging the Widgets

When you add a field, its widget will appear in the *Form Widget List*. You can edit its attributes in the *Form Widget Attributes* panel. 

- **In the *Form Widget List* panel**
  Drag and drop your widget to quickly rearrange the order of the fields.

### Previewing Your Form

Preview your form at any time using the *Preview Form* button in the top *Toolbar*. 

{{% notice tip  %}}
We recommend adding some sample data to your form before previewing. This way the form is rendered with data.
{{% /notice %}}

### Publishing Your Form

Once you've finished building the form, Click *Publish* in the top left *Toolbar*, you'll then receive a shared URL or embedding script.



##  Step 2: Uploading Your PDFs

Once you've completed the *Master Form*, it's time to upload your PDFs as *linked forms*. Use the below steps and image to guide you.

1. Click *Link* on the form you wish to add a PDF to.
2. Click *Link New PDF*, and upload the PDF.



![link-pdf](/images/link-pdf.png)



## Step 3: Editing Your Linked Form

The *Linked Form Editor* consists of two panels:

- **Left Panel**
  Displays all the widgets of the master form. You cannot add, delete, or modify the form attributes.


- **Right Panel**

  Displays the PDF form and any fields (corresponding widgets) you add to it. 

  ​

### Adding a Field to the PDF

Add a field to your PDF (in the right panel):

1. **Hover over the widget in the left panel**
2. **Click *Add to PDF***
   The field appears at the top of the PDF (right panel)
3. **Drag and Drop the field to the correct position on your PDF**

***Please Note:*** Only Text, Choice, Dropdown, and Signature can be added to a PDF form. 



![linked-form-editor-annotated](/images/linked-form-editor-annotated.png)



***Hint:*** Widgets can be added to a PDF multiple times; for example, if your PDF requires a personal signature on every page, add the same signature widget to each page. When the final PDF is generated, it will contain the same signature on every page.



### Step 4: Publishing Your Form

After you've finished building your PDF, click *Publish*. Once published, you'll receive a URL or embedding script to share.



You'll notice the sharing URL is singlular no matter how many PDFs you link, this is because the user only needs to fill out the one master form. Once the master form is complete, all the linked PDFs will automatically complete.

