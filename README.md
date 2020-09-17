# SPROUT
> #### Start a new SaaS business and cut to the chase

This is a practical guide how to get all the non-important but mandatory things out of the way as fast as possible, so you can focus on your real business value.
The goals of this guide are to:
* Be opinionated in choosing technologies and solutions so you don't have to invest too much time researching. 
* Stack is biased to towards services that have free tier so you can start with close-to-zero expenses.

Let's get strted
* [Buying a domain](#buying-a-domain)
* [Setting up brand email](#setting-up-brand-email)

### Buying a domain
Go to https://namecheap.com and search for an available domain that fit your business. Don't waste too much time on it. You can use **Beast Mode** to search across many TLDs.
If you're having hard time finding a name try https://namelix.com/ - this is a name generator that also generate logo and direct to you namecheap to register your domain. 

**Why namecheap?**
1. They are indeed cheap. Not just in the first year, also in the years to follow
2. They have great service.
3. They support most of the TLDs. 

### Setting up brand email
In order to have branded email addresses for free, we'll use 2 services. One that will forward your branded emails to your gmail inbox, and gmail itself will send out your branded emails.  
Namecheap has free email forwarding service, but it only works as long as they are the DNS provider. Since later we'll move the DNS to Cloudflare, we can't use this option. So instead we will use https://forwardemail.net/ 

**Why forwardemail?**
1. It is free. Even the premium plan is only $3/month for unlimited users
2. It is reliable
3. You can define catch-all rule
4. You can define as many addresses as you like

**Step by step:**
1. Go to https://gmail.com and sign up with a new account. I usually call it `app.YOURDOMAIN@gmail.com` 
2. Go to https://forwardemail.net/ and sign up with the gmail account you've just created
3. Define a new domain and follow the instructions to set it up. You'll have to add a TXT record in namecheap to complete the setup. Add at least the following aliases: `YOURNAME@YOURDOMAIN` `hello@YOURDOMAIN`, `support@YOURDOMAIN`. 
   * If you want you can also add a catch-all rule. Not mandatory.
   * You can forward each of your aliases to a tagged inbox in gmail using the `+` sign. For example, forward `support@YOURDOMAIN` to `app.YOURDOMIAN+support@gmail.com`. This will arrive to your gmail inbox, with the tag `support`. It can help you later if you set up any rules inside gmail.
4. Now back to gmail, you need to configure sending emails from your domain. 
   * Click the cog wheel on the upper right corner og gmail, and then click "See all settings"
   * Go to "Accounts and import"
   * The next steps you have to follow for each of the addresses you'd want to be able to use:
   * In the "Send mail as" section, click "Add another email address"
   * Put your name as it will appear to recipients, and the email address you're adding. Leave "Treat as an alias" checked. Click Next step.
   * TBC=============
   
