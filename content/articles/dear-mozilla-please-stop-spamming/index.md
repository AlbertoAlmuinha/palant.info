---
categories:
- mozilla
- email
date: "2019-04-03 19:26:47"
description: Detailing Mozilla's failures to send newsletters only to users who actually
  opted in.
lastmod: "2019-04-05 08:25:07"
title: Dear Mozilla, please stop spamming!
---

Dear Mozilla, of course I learned about your new file sharing project from the news. But it seems that you wanted to be really certain, so today I got this email:

{{< img src="mozilla_spam.png" alt="Email screenshot" width="828" />}}

Do you still remember how I opted out of all your emails last year? Luckily, I know that email preferences of all your users are managed via [Mozilla Basket](https://basket.readthedocs.io/) and I also know how to retrieve raw data. So here it is:

{{< img src="basket_data.png" alt="Screenshot of Basket data" width="415" />}}

It clearly says that I've opted out, so you didn't forget. So why do you keep sending me promotional messages? **Edit** (2019-04-05): Yes, that `optin` value is thoroughly confusing but it doesn't mean what it seems to mean. Basket only uses it to indicate a "verified email," somebody who either went through double opt-in once or registered with Firefox Accounts.

This isn't your only issue however. A year ago I reported a [security issue in Mozilla Basket](https://bugzil.la/1446612) (not publicly accessible). The essence is that subscribing anybody to Mozilla's newsletters is trivial even if that person opted out previously. The consensus in this bug seems to be that this is "working as expected." This cannot seriously be it, right?

Now there is some legislation that is IMHO being violated here, e.g. the CAN-SPAM Act and GDPR. And your privacy policy ends with the email address one can contact to report compliance issues. So I did.

{{< img src="mozilla_bounce.png" alt="Screenshot of Mozilla's bounce mail" width="957" />}}

Oh well...
