+++
title = "Export Form Submissions"
weight = 42
description = "With PlatoForms you can quickly export all your submitted forms into a CSV file."
+++
# EXPORT FORM SUBMISSIONS

Learn to export your submissions from the *submissions panel*.

* **Step 1:** Click *Export Submission*
* **Step 2:** Select a date range
* **Step 3**: Click *Export*

The file downloads as a zip file. If your form has multiple revisions, the file will include a different CSV for each revision.

The CSV file includes:
* All form data
* The generated PDF URL
* Submission date

***Please Note:*** URLs do not include the domain name. To open a URL, add the prefix https://design.platoforms.com to the given URL extension.



![export](/images/export.PNG)



Here's a description of some fields within your export:

| Field Type   | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| Choice       | The *Choice* label. If more than one is selected, they are separated by commas. If the *Other* option is used, its input value appears after the last comma. |
| Dropdown     | The *Dropdown* field can have a different label and value. Exports show the value of a *Dropdown*. If more than one is selected, they are separated by commas. |
| Signature    | A Base64 image displays the *Signature*. You can put the text as a `src` directly in the HTML img tag. |
| Upload Files | The URL for the files.  Remember to prefix your URL with `https://design.platoforms.com` |

