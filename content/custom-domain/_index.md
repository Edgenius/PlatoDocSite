+++
title = "CUSTOM DOMAIN"
description = "Learn how to use your custom domain with PlatoForms. Let your forms speak for your brand."
weight = 6
+++

{{% notice tip  %}}
If you're using our embedded forms, there is no need to set up a custom domain.
{{% /notice %}}

## Setting a Subdomain For Your Form URL

All published forms have a unique URL for access. By default, these begin with `https://forms.platoforms.com,` but you may want to use your own branded URL; you can do this with the domain masking configuration.

<div class="notices warning"><p>To set up a custom domain, you must have permission to access your domain DNS records.</p>
</div>

* **Step 1:** Login to your dashboard, and access the *Setting*s page—you can find this by clicking your name in the left column.
* **Step 2:** Click the *Custom Domain* tab in the *settings* menu
* **Step 3:** In the domain name field, type the subdomain you want to use. For example, if your domain is foo.com, you might use the subdomain form.foo.com, myform.foo.com, or any subdomain name you desire. 
* **Step 4:** Click *Update*; you'll then receive a CNAME value. You'll need this later.




![setting](/images/setting.png)



## Changing Your DNS details

Step 1: Log into your domain registrar
Step 2: Locate their DNS management
Step 3:  Add your CNAME to point it to PlatoForms

***Please Note:*** DNS management can vary between registrars, we recommend you find information about CNAME forwarding on your registrar's website or ask their support team for help.

CNAME changes can take between 24- and 48-hours to take effect.



![cname](/images/cname.png)



As soon as your CNAME record is working, your published forms will have a sharing URL specific to your custom domain name. For example, https://myform.foo.com/form/fr1srsswes. ***Remember***, the CNAME process can take 24- to 48-hours to start working. 



## Security

In many cases, your forms contain sensitive data and require HTTPS/SSL protection. We keep you secure with [Let'sEncrypt](https://letsencrypt.org/) protection—it even covers your custom domain.

We install SSL certificates as soon as your CNAME starts working. Once the installation has begun, it may take **up to four hours** before you have HTTPS protection working on your domain.



## API

Once the custom domain is set up successfully, the form URL returned by our API will be your domain URL.



## Convention URL

Even after your custom domain is working, you can still open the form with our original PlatoForms URL. To do this, replace your custom URL (https://myform.yourdomainhere.com/form/) with our PlatoForms URL (https://form.platoforms.com). Make sure you remove the `/form` from your URL—you don't need this when you use our native domain.



## CNAME Value

The CNAME value always follows the same format:

* `[subdomain].dns.platoforms.com.`

This allows you to setup CNAME before the custom domain is set.

## FAQ

**My website is www.foo.com. Is my CNAME `www.foo.com.dns.platoforms.com`?**

In most cases, no. The CNAME you use for PlatoForms must be unoccupied. If your root domain (www.foo.com) is already pointing to your website, it cannot be used for your forms, too. We suggest you create a subdomain that is unique to your forms; for example, myforms.foo.com. Your website host can help you with this.

However, if your root URL (www.foo.com) is being used solely for forms, then, yes, you can use it for PlatoForms.