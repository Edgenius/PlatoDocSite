+++
title = "Custom Domain"
description = "Set Domain Masking for your forms"
weight = 200
+++

## Set Subdomain for your form URL 
After you publish the form, it has a unique URL to open this form. By default, it is starting with `https://forms.platoforms.com`. In some cases, you may want to hide `platoforms.com` from your customers. You can achieve this by the domain masking configuration. 

{{% notice warning  %}}
To setup custom domain, you must have the permission to update your domain DNS records!
{{% /notice %}}

The first step is login our dashboard, go to `settings` page (under the avatar at the top left corner, click your name), then go to "Custom Domain" tab. In domain name field, input the subdomain you want to use to open the form. For example, if your domain is `foo.com`, you may uses `form.foo.com`, `myform.foo.com`, `form.sales.foo.com` or any meaningful subdomain name.  After you press the `Update` button, you will get a CNAME value. 

![Settings](/images/page/domains/setting.png)

As the example, here uses Godday as your domain registrar. Log into Godaddy, goes to DNS management from it domain manage panel, then click "Add".  At `Type` field, choose `CNAME`, input the subdomain name (exclude your root domain) i.e, `myform` as `Host` value.  At `Points to`, input our CNAME value, i.e., `myform.foo.com.dns.platoforms.com`.  Save and exit.  Note, this CNAME change could take up-to-24 hours to broadcast over the Internet. 

![Godaddy CNAME](/images/page/domains/cname.png)


Once your CNAME record is working, your published form will get a sharing URL by your domain, for instance, `https://myform.foo.com/form/fr1srsswes`. However, as mentioned above, this URL only takes effect until your CNAME is valid across the Internet. Just be patient, if it doesn't work after 24 hours, please double check your DNS settings or contact our support. 


## Security

Your form submission may contain sensitive data so the HTTPS / SSL protection is very essential. We issue HTTPS and SSL certification from [Let'sEncrypt](https://letsencrypt.org/), it is automatically installed and renewed for your custom domain! The SSL certification installation relies on your CNAME settings in domain registrar. Only the CNAME starts working, our system scheduler can trigger the SSL installation. This could take up-to-4 hours to enable the HTTPS protection. 


## API

Once the custom domain set up successfully, the form URL returned from our API will be your domain URL. 


## Convention

#### URL
Even you setup the custom domain, you still can open the form by our URL.  You just manually replace `https://myform.yourdomainhere.com/form/` with our form domain URL "https://form.platoforms.com".  Please be careful, in your custom domain URL, it has `/form` in the middle of URL, but ours doesn't have.  For example, `https://myform.yourdomainhere.com/form/fr1srsswes` will be `https://form.platoforms.com/fr1srsswes`. 


#### CNAME Value

Our CNAME value is always in `your-subdomain.dns.platoforms.com` format, i.e., suffix with `.dns.platoforms.com`.  This means you even can setup CNAME before our custom domain setting. 


