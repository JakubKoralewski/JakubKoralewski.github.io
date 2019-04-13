# How to setup e-mail using a custom domain for free (Github Student Developer Pack + Namecheap + SendGrid + Gmail)

[medium-article]: https://medium.com/issacaption/using-a-custom-domain-in-gmail-for-free-with-mailgun-and-sendgrid-2c54e681f378
[student-pack]: https://education.github.com/pack

This is adapted from [this Medium article][medium-article] by Nathan H. Leung. The major difference is that he used MailGun to receive e-mails, and SendGrid to send them. Instead I use NameCheap to receive them, but SendGrid is used in the exact same way!
<hr/>
&nbsp;

## Get your [Github Education][student-pack] package

1. From your GitHub Student Developer Pack get:
   1. your free `.me` domain from Namecheap.
   2. your free SendGrid account.
<hr/>
&nbsp;

## Receive e-mails to your custom domain

In your Namecheap domain's settings go to the Domain tab. Go to the `REDIRECT EMAIL` section and set the Catch-All Alias to your private e-mail address.

![](https://i.imgur.com/OQtrW62.png)
*Listing 1: Redirect any email to \*@yourdomain.me to your private e-mail address*.
&nbsp;

Now any e-mail to your custom domain will get redirected to your e-mail. In Gmail they will appear as if they were sent to the targeted domain, e.g.: `kontakt@jcubed.me` not your e-mail address you forward your e-mail to.

But `how to send e-mails, j³?`, you may ask.
<hr/>
&nbsp;

## How to send e-mails

Remember you have a SendGrid account. This is where it comes into play. This part is the same as in [the Medium article][medium-article] by Nathan H. Leung. The only difference is he used a trial account in his example, but you have 15000 e-mails per month for free while you're a student thanks to your [Github Student Developer Pack][student-pack]! Check out his full description in the article or use my shortened list here:

1. Open your SendGrid account.
2. Open your API key settings [here](https://app.sendgrid.com/settings/api_keys).
   1. Hit the `Create API Key` button.
   2. Save your API Key somewhere. You won't see it again.
3. Go to your Gmail settings.
   1. Go to the `Accounts and Import` tab.
   2. Then to the `Send mail as:` section.
   3. Add a new account.
   
Here's a crazily awesome snippet Nathan has found. It's tremendously useful.

```
SMTP Server: smtp.sendgrid.net
Username: apikey
Password: <your api key from step 3>
```
*Listing 2: How to set the SMTP settings in your Gmail settings*
&nbsp;

The username is `apikey` and the password is your actual API Key. This is an awesome find, because it's not something SendGrid actively advertises you can do, but Nathan found it in SendGrid's API docs [here](https://sendgrid.com/docs/API_Reference/SMTP_API/getting_started_smtp.html)!
<hr/>
&nbsp;

## That's it!

Free `.me` domain for a year. Free 15000 e-mails per month thanks to SendGrid. The combination of both lets me put this here:

contact@jcubed.me
<hr/>
&nbsp;
&nbsp;

## Sources

Again, much respect to Nathan H. Leung for his awesome article:

[https://medium.com/issacaption/using-a-custom-domain-in-gmail-for-free-with-mailgun-and-sendgrid-2c54e681f378][medium-article]