#emailGrid

##An email newsletter grid template

emailGrid is a starting point for creating a bulletproof email template. You take what you want and run with it. It is designed to be as email service agnostic as possible. I’ve used it plenty with [Campaign Monitor](http://www.campaignmonitor.com) and [MailChimp](http://mailchimp.com). 

Tables, tables, tables! Tables is stable, and we need to kick it oldschool for email newsletters. Fortunately, I lived through the browser wars of the mid 90s, and these are the best practices I cut my teeth on!

##Features

* 600px width. The maximum allotted space for your messaging with respectable gutters.
* 1, 2, 3, and 6 column widths, including “floated image” columns (you can’t float in emails, son).
* Share on Facebook, Twitter and Email using nothing more than old-fashioned URLs.
* Namespaced find/replace placeholder variables to make customizing a little easier on you. If you host your newsletters on your website, you can replace these with real variable from your favorite server-sided language.
* Email client preview pane text. “Having trouble viewing this email?” Probably not. Don’t let this be the message everyone sees in their iPhone mail listing.

##Find/Replace Placeholder Variables

* [eG-newsletterTitle] - The name of your newsletter
* [eG-issueTitle] - The subject of the email
* [eG-previewText] - Text to display in the preview pane of mobile devices and email clients
* [eG-issueUrl] - The URL of the email on your web server with protocol and trailing slash. Ex. http://yourdomain.com/newsletter/01-01/
* [eG-issueImg] - Image to use for sharing on Facebook
* [eG-twitterName] - The Twitter user name of the organization 
* [eG-orgName] - The actual, real name of your organization (required by US law)
* [eG-streetAddress] - The actual, real mailing address/P.O. Box of your organization (required by US law)
* [eG-siteUrl] - The URL of your organization website without http:// 

###Email Service Placeholder Variables

* [eG-unsubscribe] = Campaign Monitor: \<unsubscribe>opt-out\</unsubscribe> MailChimp: \<a href="*|UNSUB|*">opt-out\</a> (required by US law)
* [eG-subscriberEmail] = Campaign Monitor: [email] MailChimp: \*|EMAIL|*

It’s in a usable state now, but watch for updates in the coming weeks. I’m about to run it through some rigorous testing.

