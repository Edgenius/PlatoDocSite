+++
title = "Workflow Step Settings"
description = "Workflow Step Settings"
weight = 200
+++

The working flow step settings are used for PDF creation and form display after the first step.

{{% notice tip  %}}
<a name="HM-WORKFLOW-010" class="anchor"></a>
This form submission will print on the PDF that is created in last step. 
{{% /notice %}}

As an example, the first step is customer filled information. In this PDF, you also need to put your signature to approve the deal. With this option, the final PDF will combine the customer's information and your signature.  Note, our system doesn't check if this step is using the same PDF with the previous step. 

{{% notice tip  %}}
<a name="HM-WORKFLOW-015" class="anchor"></a>
If your form is a PDF Online Form, you can use the previous step created PDF as this form template.
{{% /notice %}}

As an example, this form template in this step is the PDF that customer filled out in the first step, so the sales manager can easily understand what they approved for.

{{% notice tip  %}}
<a name="HM-WORKFLOW-020" class="anchor"></a>
A link on the bottom of the form to open the PDF that is created in the last step. This is helpful if your form is not PDF Online Form or the 2nd option is turned off. 
{{% /notice %}}

This needs the `Form Submission Viewer` permission on your previous step form. If you got an access denied error (HTTP 403), you need to check if you logged into PlatoForms if you don't set the last form Submission Viewer permission to `Public`. 


{{% notice tip  %}}
<a name="HM-WORKFLOW-025" class="anchor"></a>
A link on the bottom of your form to open the form that is filled in last step. It gives a chance to modify previous submission. 
{{% /notice %}}

This needs the `Form Submitter` permission on your previous step form. If you got an access denied error (HTTP 403), you need check if you logged into PlatoForms if you don't set the last form Submitter permission to `Public`. 
