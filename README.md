# Google Dorks for Bug Bounty

A list of Google Dorks for Bug Bounty, Web Application Security, and Pentesting

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/TakSec.svg?style=social&label=Follow%20%40TakSec)](https://twitter.com/TakSec)
</p>

---

### Broad domain search w/ negative search

> site:example.com -www -shop -share -ir -mfa

### Code leaks

> site:pastebin.com "example.com"

> site:jsfiddle.net "example.com"

> site:codebeautify.org "example.com"

> site:codepen.io "example.com"

### PHP extension w/ parameters

> site:example.com ext:php inurl:?

### Disclosed XSS and Open Redirect Bug Bounties

> site:openbugbounty.org inurl:reports intext:"example.com"

### File upload endpoints

> site:example.com ”choose file”

### Cloud Storage

> site:s3.amazonaws.com "example.com"

> site:blob.core.windows.net "example.com"

> site:googleapis.com "example.com"

> site:drive.google.com "example.com"

> site:dev.azure.com "example[.]com"

> site:onedrive.live.com "example[.]com"

> site:digitaloceanspaces.com "example[.]com"

> site:sharepoint.com "example[.]com"

> site:s3-external-1.amazonaws.com "example[.]com"

> site:s3.dualstack.us-east-1.amazonaws.com "example[.]com"

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

### WordPress

> inurl:/wp-admin/admin-ajax.php

### Drupal

> intext:"Powered by" & intext:Drupal & inurl:user

### Joomla

> site:*/joomla/login

### XSS prone parameters

> inurl:q= | inurl:s= | inurl:search= | inurl:query= inurl:& site:example.com

### Open Redirect prone parameters

> inurl:url= | inurl:return= | inurl:next= | inurl:redir= inurl:http site:example.com

### Apache Server Status Exposed

> site:*/server-status apache

### JFrog Artifactory

> site:jfrog.io "example[.]com"

### Firebase

> site:firebaseio.com "example[.]com"


---

Medium articles for more dorks:

https://thegrayarea.tech/5-google-dorks-every-hacker-needs-to-know-fed21022a906

https://infosecwriteups.com/uncover-hidden-gems-in-the-cloud-with-google-dorks-8621e56a329d
