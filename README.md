#emailGrid

##An email newsletter grid template

emailGrid is a starting point for creating a bulletproof email template. You take what you want and run with it. It is designed to be as email service agnostic as possible. I’ve used it plenty with [Campaign Monitor](http://www.campaignmonitor.com) and [MailChimp](http://mailchimp.com). 

Tables, tables, tables! Tables is stable, and we need to kick it oldschool for email newsletters. Fortunately, I lived through the browser wars of the mid 90s, and these are the “best practices” I cut my teeth on!

Remember, the majority of the structure is in the markup. Everything is based on a 80px grid with 10px of padding on each side. This leaves a 100px grid that includes 20px gutters between columns, and 10px gutters on the sides of the email.

<table>
	<thead>
		<tr>
			<th>If you want ...</th>
			<th>Set td width attr to ...</th>
		</tr>
	</thead>
	
	<tbody>
		<tr>
			<td>600px</td>
			<td>580px</td>
		</tr>
		<tr>
			<td>400px</td>
			<td>380px</td>
		</tr>
		<tr>
			<td>200px</td>
			<td>180px</td>
		</tr>
		<tr>
			<td>100px</td>
			<td>80px</td>
		</tr>
	</tbody>
</table>

##Features

* 600px width. The maximum recommended space for your messaging with respectable gutters.
* 1, 2, 3, 4 and 6 column widths, including “floated image” columns (you can’t float in emails, son).
* Share on Facebook, Twitter and Email using nothing more than old-fashioned URLs.
* Find/replace placeholder text to make customizing a little easier on you. If you host your newsletters on your website, you can replace these with  variables from your favorite server-sided language.
* Email client preview pane text. “Having trouble viewing this email?” Probably not. Don’t let this be the message everyone sees in their iPhone mail listing. Set it in the markup, and hide it with CSS.
* All style classes and placeholder text is namespaced with “eG-” for easy customizability.

##Find/Replace Placeholder Text

* [eG-newsletterTitle] - The name of your newsletter
* [eG-issueTitle] - The subject of the email
* [eG-previewText] - Text to display in the preview pane of mobile devices and email clients (hidden with CSS)
* [eG-issueUrl] - The URL of the email on your web server with protocol and trailing slash. Ex. http://yourdomain.com/newsletter/01-01/
* [eG-issueImg] - Image to use for sharing on Facebook
* [eG-twitterName] - The Twitter user name of the organization 
* [eG-orgName] - The actual, real name of your organization (required by US law)
* [eG-streetAddress] - The actual, real mailing address/P.O. Box of your organization (required by US law)
* [eG-siteUrl] - The URL of your organization website without http:// 

###Email Service Placeholder Variables

* [eG-unsubscribe] = Campaign Monitor: \<unsubscribe>opt-out\</unsubscribe> MailChimp: \<a href="\*|UNSUB|\*">opt-out\</a> (required by US law)
* [eG-subscriberEmail] = Campaign Monitor: [email] MailChimp: \*|EMAIL|\*

