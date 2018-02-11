+++
title = "Workflow Step Settings"
description = "Workflow Step Settings"
weight = 200
+++

The working flow step settings are used for PDF creation and form display after the first step.

{{% notice tip  %}}
<a name="HM-WORKFLOW-010" class="anchor"></a>
This form submission will print on previous step generated PDF.
{{% /notice %}}


As an example, the first step is customer filled information. In this PDF, you also need to put your signature to approved the deal. With this option, the final PDF will combine the customer's information and your signature.  Note, our system doesn't check if this step is using same PDF with previous step, as we want to give your maximum flexible to design the workflow. 

{{% notice tip  %}}
<a name="HM-WORKFLOW-015" class="anchor"></a>
If your form is an PDF Online Form, with this option, you can use previous step created PDF as this form template.
{{% /notice %}}

As an example, this form template in this step is the PDF that customer filled out in first step, so the sales manager can easily understand what they approved for.

{{% notice tip  %}}
<a name="HM-WORKFLOW-020" class="anchor"></a>
A link on the bottom of the form to open the last step generated PDF. This is helpful if your form is not PDF Online Form or you don't turn on above 2nd option. 
{{% /notice %}}

This needs the `Form Submission Viewer` permission on your previous step form. If you got an access denied error (HTTP 403), you need to check if you logged into PlatoForms if you don't set the last form Submission Viewer permission to `Public`. 


{{% notice tip  %}}
<a name="HM-WORKFLOW-025" class="anchor"></a>
A link on the bottom of your form, it opens the last step form with data in a new window. It gives a chance to modify last step filled data. 
{{% /notice %}}

This needs the `Form Submitter` permission on your previous step form. If you got an access denied error (HTTP 403), you need check if you logged into PlatoForms if you don't set the last form Submitter permission to `Public`. 
