+++
title = "WORKFLOW STEP SETTINGS"
description = "Have full control over your workflow. PlatoForms lets you customise every step of the process."
weight = 205
+++

Once the first step is in place, the workflow steps have settings to help you control and display the form.

Workflow settings (only available for step two and beyond):

![workflow-step-settings](/images/workflow-step-settings.png)

- **Merge the submission content with the previously created PDF**

{{% notice tip  %}}
<a name="HM-WORKFLOW-010" class="anchor"></a>
This form submission will print on the PDF that is created in the last step.
{{% /notice %}}


  Use this option to combine multiple steps onto the same PDF. 

  For example, in step one a customer enters their personal information; but on this page of the PDF, we also need the sales manager's signature—this is Step 3. By enabling this option, the PDF will merge both steps onto the same page, showing both the customer's information and the manager's signature on the final generated PDF.


- **Use previously created PDF as current form template**


{{% notice tip  %}}
<a name="HM-WORKFLOW-015" class="anchor"></a>
If you're using a PDF Online Form, you can use the PDF created after the previous step was completed as your new form template.
{{% /notice %}}

  Enabling this option will display the previous step's information on the PDF. This allows the user to reference preceding information while filling out the form. For example, a sales manager will be able to reference a sales form and know what they are signing. 
  ​

- **Show the PDF link of previous step**


{{% notice tip  %}}
<a name="HM-WORKFLOW-020" class="anchor"></a>
A link at the bottom of your form that opens the PDF generated after the previous step. This is helpful if your form is not a PDF Online Form, or you have 'Use previously created PDF as current form template' turned off.
{{% /notice %}}


  Turning on this option displays a link to the PDF created **after** the previous step was completed. This is useful if your form is not a PDF Online Form, or have turned off *Use previously created PDF as current form template.

  Use this option if you need to reference the previous steps details, but don't want to have them showing on the current PDF template. 


- **Show the form link of previous step**

{{% notice tip  %}}
<a name="HM-WORKFLOW-025" class="anchor"></a>
A link at the bottom of your form to open the previous step's filled in form; this allows you to modify an earlier submission.
{{% /notice %}}

  This option displays a link at the bottom of the form to open the form of the previous step. This is useful if you might need to change information submitted in the earlier steps.

  ***Please Note:*** This option needs the *Form Submitter* permission on the previous step's form. If you receive an access denied error (HTTP 403), check that you are logged-in to PlatoForms and set the previous form's *Form Submitter* permission to *Public*.




