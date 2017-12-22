# Testphp_vulns
Collect all vulns and infomations in http://testphp.vulnweb.com/

## Sensitive Files

    http://testphp.vulnweb.com/index.zip
    http://testphp.vulnweb.com/.idea/workspace.xml
    http://testphp.vulnweb.com/admin/
    http://testphp.vulnweb.com/Mod_Rewrite_Shop/.htaccess
    http://testphp.vulnweb.com/crossdomain.xml
    http://testphp.vulnweb.com/CVS/Root
    http://testphp.vulnweb.com/secured/phpinfo.php
    

## Directory Index

    http://testphp.vulnweb.com/Flash/
    http://testphp.vulnweb.com/CVS/
    http://testphp.vulnweb.com/.idea/
  
## Infomation disclosure
  
    wvs@acunetix.com
    test@gmail.com
    http://127.0.0.1
    wasp@acunetix.com
  
## XSS
  
    POST http://testphp.vulnweb.com/search.php 'searchFor'
    POST http://testphp.vulnweb.com/guestbook.php 'name'
    POST http://testphp.vulnweb.com/secured/newuser.php 'uuname'
   
  
## SQL Inject

    POST http://testphp.vulnweb.com/secured/newuser.php 'uuname' error SQLi vulnerable
    POST http://testphp.vulnweb.com/userinfo.php 'uname' blind SQLi vulnerable
  
## File Include

## CLRF

## Weak Pass

    test/test
