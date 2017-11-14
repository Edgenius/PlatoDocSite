+++
title = "Export Form Submissions"
weight = 30
description = "Export Form Submissions Data with CSV files"
+++


Press `Export submission` button, select a date range to set the scope for a submitted date. The download is starting after a while by clicking `Export` button. 

The download is zipped file. If this form has multiple revisions, i.e, you have published this form multiple times, the zip will include the different CSV for each revision of this form.  

All form data is included in CSV file, more than that, it also includes the generated PDF URL and submitted date. The URL does not include the domain name. To open the URL, you need to add prefix `https://design.platoforms.com` over the given URL. 

![Export Submission](/images/page/submission/export.png)


Here is the detail description of some special fields:

Field Type    | Description
--------|------
Choice |  The label of Choice.  If multiple selected, they are separated by a comma. If it has `Other Option`, the other input value is after the last comma.
Dropdown | Note, Dropdown field can have different label and value. The export is the value of Dropdown. If multiple selections, they are separated by a comma.
Signature | [Base64 image image](https://en.wikipedia.org/wiki/Data_URI_scheme). You can put the text as src directly in HTML img tag.
Upload Files | The part of URL after `https://design.platoforms.com`

