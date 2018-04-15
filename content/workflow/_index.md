+++
title = "Workflow"
description = "Workflow"
weight = 2
+++

{{% notice tip  %}}
<a name="HM-WORKFLOW-100" class="anchor"></a>
In a workflow, the PDF can be filled out in multiple steps. 
{{% /notice %}}


To explain what is workflow, let's start with a use case. For example,  a car sale form needs to be filled out both customer and the salesman. It may also need the sale manager's signature. With PlatoForms, you can build a workflow to achieve this. The workflow includes multiple forms, we call each form as a `Step`.  A workflow can include any amount of steps. Once a form is filled out, an email notification is sent to the correspondents where includes a link to next step. In most cases, the form of each step could use the same PDF. The submission data is overlapping to the PDF of its previous step created. Think about above use case, it may include 3 steps in a workflow to complete this sale form. The first step is for the customer where they filled the personal information, e.g, family name, address or phone etc. The second form is for the salesman who will fill out the information of the car. In the final step, it is for the sales manager who will sign on the form. All forms in these 3 steps are pointing to the same PDF, ie., that sale form. They got a completion PDF with all necessary information after the last step is submitted. 

Workflow can be more flexible by different settings. For example, you can decide if the current step data overlap to previous step PDF. You can mix different form types, i.e, web online form or PDF online form. Still, for above example, the first 2 steps could be designed in web online form format. It is easier for your customer and salesman.  The last step for sales manager can use PDF online form. The background of form is just that PDF with all customer and salesman information so the manager is able to review and decide to sign or revise it easily. In workflow, you even can use different PDF files per step.

