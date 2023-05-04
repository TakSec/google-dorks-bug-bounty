# Google Dorks for Bug Bounty

A list of Google Dorks for Bug Bounty, Web Application Security, and Pentesting

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/TakSec.svg?style=social&label=Follow%20%40TakSec)](https://twitter.com/TakSec)
</p>

---

### Broad domain search w/ negative search

> site:example.com -www -shop -share -ir -mfa

### PHP extension w/ parameters

> site:example.com ext:php inurl:?

### Disclosed XSS and Open Redirects

> site:openbugbounty.org inurl:reports intext:"example.com"

### Juicy Extensions

> site:"example[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess | ext:xml | ext:reg | ext:inf | ext:rdp | ext:cfg | ext:txt | ext:ora

### Directory Listing

> site:example.com intitle:index.of

### Exposed Database Files

> site:example.com ext:sql | ext:dbf | ext:mdb

### Wordpress

> site:example.com inurl:wp- | inurl:wp-content | inurl:plugins | inurl:uploads | inurl:themes | inurl:download

### Find Login Pages

> site:example.com inurl:login

### BackUp and Old Files

> site:example.com ext:bkf | ext:bkp | ext:bak | ext:old | ext:backup

### Sql Errors

> site:example.com intext:"sql syntax near" | intext:"syntax error has occurred" | intext:"incorrect syntax near" | intext:"unexpected end of SQL command" | intext:"Warning: mysql_connect()" | intext:"Warning: mysql_query()" | intext:"Warning: pg_connect()"

### Exposed Documents

> site:example.com ext:doc | ext:docx | ext:odt | ext:pdf | ext:rtf | ext:sxw | ext:psw | ext:ppt | ext:pptx | ext:pps | ext:csv

### Install / Setup Files

> site:example.com inurl:readme | inurl:license | inurl:install | inurl:setup | inurl:config

### Open Rediects

> site:example.com inurl:redir | inurl:url | inurl:redirect | inurl:return | inurl:src=http | inurl:r=http

### Code Leaks

> site:pastebin.com "example.com"

> site:jsfiddle.net "example.com"

> site:codebeautify.org "example.com"

> site:codepen.io "example.com"

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

> site:dropbox.com/s "example[.]com"

> site:box.com/s "example[.]com"

> site:docs.google.com inurl:"/d/" "example[.]com"

### XSS prone parameters

> inurl:q= | inurl:s= | inurl:search= | inurl:query= inurl:& site:example.com

### Open Redirect prone parameters

> inurl:url= | inurl:return= | inurl:next= | inurl:redir= inurl:http site:example.com

### SQLi Prone Parameters

> inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:example.com

### SSRF Prone Parameters

> inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:example.com

### LFI Prone Parameters

> inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:example.com

### RCE Prone Parameters

> inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:example.com

### High % inurl keywords

> inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:example[.]com

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:example[.]com

### JFrog Artifactory

> site:jfrog.io "example[.]com"

### Firebase

> site:firebaseio.com "example[.]com"

### API Docs

> inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"example[.]com"

### File upload endpoints

> site:example.com ”choose file”

## Dorks that work better w/o domain

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

> site:*/security.txt "bounty"

### Apache Server Status Exposed

> site:*/server-status apache

### WordPress

> inurl:/wp-admin/admin-ajax.php

### Drupal

> intext:"Powered by" & intext:Drupal & inurl:user

### Joomla

> site:*/joomla/login

---

Medium articles for more dorks:

https://thegrayarea.tech/5-google-dorks-every-hacker-needs-to-know-fed21022a906

https://infosecwriteups.com/uncover-hidden-gems-in-the-cloud-with-google-dorks-8621e56a329d

https://infosecwriteups.com/10-google-dorks-for-sensitive-data-9454b09edc12

Top Parameters:

https://github.com/lutfumertceylan/top25-parameter

Proviesec dorks:

https://github.com/Proviesec/google-dorks
