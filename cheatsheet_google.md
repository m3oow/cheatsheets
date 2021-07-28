# Google dorks cheatsheet

## Table of contents

* [Interesting sources](#_sources)
* [Dorks 1](#_d1)
* [Dorks 2](#_d2)

## Interesting sources <a name="_sources"></a>

https://www.exploit-db.com/google-hacking-database

## Dorks 1 <a name="_d1"></a>

```
inurl:"/vpn/tmindex.html" vpn
intext:"Powered by GetSimple" -site:get-simple.info
inurl:"/fuel/login"
intitle:"index of" intext:"Includes wordpress"
intitle:"netscaler gateway" intext:password "please log on"
inurl:users.json + "username"
intitle:"index of" intext:"Includes
inurl:old "index of" "wp-config.php"
inurl:9000 AND intext:"Continuous Code Quality"
s3 site:amazonaws.com filetype:sql
intext:"wordpress" filetype:xls login & password
"Web Analytics powered by Open Web Analytics - v: 1.6.2"
intitle:"Outlook Web Access" | "Outlook Web app" -office.com -youtube.com -microsoft.com
intext:"Sign in with your organizational account" login -github.com
"/FTPSVC2" intitle:"index of"
intitle:"index of" "W3SVC1"
inurl:"CookieAuth.dll?GetLogon?" intext:log on
-youtube.com login | password | username intitle:"assessment"
s3 site:amazonaws.com filetype:xls login
s3 site:amazonaws.com filetype:xls password
intext:backup.sql intitle:index.of
intext:user.sql intitle:index.of
inurl:jsmol.php
intitle:"Pi-hole Admin Console"
filetype:inc php -site:github.com -site:sourceforge.net
filetype:php "Notice: Undefined variable: data in" -forum
intitle:"WAMPSERVER homepage" "Server Configuration" "Apache Version"
intitle:"report" ("qualys" | "acunetix" | "nessus" | "netsparker" | "nmap") filetype:pdf
filetype:git -github.com inurl:"/.git"
intitle:"iLO Login" intext:"Integrated Lights-Out 3"
filetype:svn -gitlab -github inurl:"/.svn"
"please sign in" "sign in" "gophish" +"login"
intitle:"LaserJet" "Device status" "Supplies summary"
inurl:github.com intext:.ftpconfig -issues
inurl:bc.googleusercontent.com intitle:index of
intitle:"admin console" inurl:login site:"*.edu"|site:"*.gov"|site:"*.net" -site:*.com -help -guide -documentation -release -notes -configure -support -price -cant
inurl:/login.rsp
site:global.gotomeeting.com inurl:recording
inurl:/web-console/ServerInfo.jsp | inurl:/status?full=true
inurl:/CFIDE/administrator/index.cfm | inurl:/CFIDE/componentutils/login.cfm | inurl:/CFIDE/main/ide.cfm | inurl:/CFIDE/wizards/
intitle:"oracle bi publisher enterprise login"
"keyed alike" site:gov filetype:pdf
inurl:"/Shop/auth/login"
inurl:office365 AND intitle:"Sign In | Login | Portal"
intext:"Login | Password" AND intext:"Powered by | username" AND intext:Drupal AND inurl:user
intext:"config" intitle:"Index of .ssh"
"php class JConfig" AND inurl:configuration AND ext:"bak | old | pdf | php | txt"
inurl:"urlstatusgo.html?url=" -intext:"Disallowed by URL filter"
inurl:"cs.html?url="
inurl:+CSCOE+/logon.html
inurl:login.txt filetype:txt
inurl:login.aspx filetype:aspx intext:"TMW Systems"
jmeter.log filetype:log
intitle:settings.py intext:EMAIL_USE_TLS -git -stackoverflow
inurl:wp-config.php intext:DB_PASSWORD -stackoverflow -wpbeginner
intext:"@gmail.com" AND intext:"@yahoo.com" filetype:sql
intext:"the WordPress" inurl:wp-config ext:txt
site:mil ext:cfm inurl:login.cfm
"passport" filetype:xls site:"*.edu.*" | site:"*.gov.*" | site:"*.com.*" | site:"*.org.*" | site:"*.net.*" | site:"*.mil.*"
site:connect.garmin.com inurl:"/modern/profile/"
site:connect.garmin.com inurl:"/modern/activity/"
intitle:"qBittorrent Web UI" inurl:8080
intext:"series Network Configuration" AND intext:"canon"
inurl:ctl/Login/Default.aspx
inurl:dnn.js
inurl:TOP/PRTINFO.HTML
intitle:"index of" scada
inurl:/clusters intitle:"kafka Manager"
inurl:7474/browser intitle:Neo4j
intitle:OmniDB intext:"user. pwd. Sign in."
intext:"Powered by 74cms v5.0.1"
inurl:wp-login.php?action=register
intext:[To Parent Directory] & ext:sql | ext:cnf | ext:config | ext:log
ext:txt | ext:sql | ext:cnf | ext:config | ext:log & intext:"admin" | intext:"root" | intext:"administrator" & intext:"password" | intext:"root" | intext:"admin" | intext:"administrator"
inurl:/pages/default.aspx | inurl:/páginas/default.aspx
site:www.openbugbounty.org + intext:"Open Redirect" + intext:"Unpatched"
"Powered by ViewVC 1.0.3"
"/var/cache/registry/"
inurl:_vti_bin/sites.asmx?wsdl | intitle:_vti_bin/sites.asmx?wsdl
type:mil inurl:ftp ext:pdf | ps
site:com inurl:b2blogin ext:cfm | jsp | php | aspx
site:com inurl:jboss filetype:log -github.com
inurl:/signin.php?ret=
"This service is powered by a copy of ZendTo"
allintitle: "index of/admin"
intitle: "index of" "./" "./bitcoin"
intitle:"index of" ".cpanel/caches/config/"
intitle: "Index of" intext:log
Find 3cx Phone System Management Console
intitle:"Directory Listing For" "Filename" intext:Tomcat/5.0.28
site:azurewebsites.net inurl:.gov | .mil | .edu
intitle: "index of" "includes"
inurl:/uploads/wc-logs/
intitle:"index of" "db"
intitle:"iDRAC-login"
intitle:"Log In - Juniper Web Device Manager"
intitle:.:: Welcome to the Web-Based Configurator::.
"Powered by BOINC"
"Powered by Trac 1.0.2"
"online learning powered by bksb"
inurl:/php-errors.log filetype:log
inurl:/files/_log/ filetype:log
inurl:8000/portal/
inurl:/portal/apis/fileExplorer/
inurl:'/scopia/entry/index.jsp'
inurl:'/logon/logonServlet'
intitle:'Welcome to JBoss AS'
inurl:'/zabbix/index.php'
intitle:'Centreon - IT & Network Monitoring'
"/1000/system_information.asp"
inurl:typo3conf/l10n/
inurl:/files/contao
/adp/self/service/login
intext:reports filetype:cache
intitle:"NetcamSC IP Address"
inurl:/phpMyAdmin/setup/index.php?phpMyAdmin=
inurl:pipermail filetype:txt
intitle:"index of" ".dockerignore"
intitle:"index of" "/aws.s3/"
inurl:SSOLogin.jsp intext:"user"
intitle:settings.py intext:EMAIL_HOST_PASSWORD -git -stackoverflow
intitle:"index of" "/bitcoin/"
intitle:"index of" ".pem"
allinurl:asdm.jnlp
inurl:/snap.cgi?&-getpic
intitle:"Home-CUPS" intext:printers -mugs
"Last modified" intitle:"index of" "dropbox"
"description" & "size" intitle:"index of" "owncloud"
"sasl_passwd" | smtpd.conf intitle:"index of"
intitle:"index of" "/user" | "/users"
username | password inurl:resources/application.properties -github.com -gitlab
intitle:"index of" hosts.csv | firewalls.csv | linux.csv | windows.csv
intitle:"index of" users.csv | credentials.csv | accounts.csv
inurl:scanned & documents intitle:"index of" IT
intitle:"index of" inurl:documents backup
intitle:vendor | supply & login | portal intext:login | email & password
intext:pin | userid & password intitle:supplier | supply & login | portal
allinurl:"/SilverStream/Meta/"
inurl:/za/login.do
inurl:/adfs/services/trust
intitle:rms webportal
inurl:F5Networks-SSO-Req?
inurl:shared/login.jsp?/ BMC arsys
inurl:login.htm "xpress" password
inurl:login.htm "access" database
"Proudly created with Wix.com"
inurl:"/cgi-bin/WS_FTP.LOG"
inurl:"/cgi-bin/CVS/"
inurl:"/.Trash" intitle:"index of" ~
intitle:"index of" $Recycle.bin
intitle:"index of" "/Windows/Recent" | "/Windows/History/"
intitle:"index of" "WindowsCookies"
intitle:"index of" "Application Data/Microsoft/Credentials"
intitle:"index of" "hiberfil.sys"
allintitle:"Index of /Admin/Common" | allintext:"Parent Directory"
allinurl:"wp-content/plugins/wordpress-popup/views/admin/"
inurl:"/my-account-login" | allintext:"My Account"
allintitle:"Index of /ThinkPHP" | inurl: "/ThinkPHP/"
inurl:nagios/cgi-bin/status.cgi
inurl:/FxCodeShell.jsp/ "Login Form" "Blog Comments"
intext:"Portador do CPF"
inurl:"/sidekiq/busy"
intitle:"Device(" AND intext:"Network Camera" AND "language:" AND "Password"
intext:"Any time & Any where" AND "Customer Login"
intitle:"Screenly OSE" intext:"Schedule Overview" AND "Active Assets" AND "Inactive Assets"
inurl:"fhem.cfg" AND 'fhem.cfg' -github
intitle:"InfluxDB - Admin Interface" -github
intitle:"webcam 7" inurl:'/gallery.html'
intitle:"Login - Xfinity" AND "Gateway > Login"
intitle:QueryService Web Service
intitle:"index of /" ssh
"Please click here to download and install the latest plug-in. Close your browser before installation."
inurl:/pwm/public/
inurl:/login.zul
intitle:"FCKeditor - Uploaders Tests"
intitle:"FCKeditor - Connectors Tests"
inurl:/setup.cgi@next_file=
intitle:"Index of /" inurl:passport
intext:" - 2019 Cott Systems, Inc."
"I have been invoked by servletToJSP"
inurl:/sap/bc/bsp
inurl:/irj/portal
inurl:/scripts/wgate
inurl:infoviewapp
inurl:"/irj/go/km/docs/"
inurl:"/irj/go/km/" intext:navigation
inurl:"/webdynpro/resources/sap.com/"
filetype:cwr inurl:apstoken
inurl:apspassword
filetype:pub "ssh-rsa"
filetype:doc "Answer Key"
inurl:"ai1wm-backups"
"dispatch=debugger."
intitle:Test Page for the Nginx HTTP Server on Fedora
inurl:admin.php inurl:admin ext:php
intitle: "Nexus Repository Manager"
inurl:LOG.txt X-System folder
inurl:webman/index.cgi
"Example: jane.citizen1"
intext:"EQ1PCI"
intext:password "Login Info" filetype:txt
filetype:txt "Registration Code"
"login":
inurl:_cpanel/forgotpwd
"Powered by vShare"
inurl:/help/lang/en/help
inurl:public.php inurl:service ext:php
filetype:xml config.xml passwordHash Jenkins
intitle:ProFTPD Admin - V1.04
intitle:"VB Viewer"
index of /etc/certs/
intitle:"Index of /private/"
"inurl:"Umbraco/#/login" site:*edu"
"site:ghostbin.com " / " "
"site:hastebin.com " / " "
intitle:'index of' "error_log"
intitle:'index of' "access_log"
inurl:/certsrv/certrqus.asp
inurl:/config/authentication_page.htm
intext:"Type in Username and Password, then click Ok" intitle:"log in"
intitle:"index of /" intext:/backup
"syd_apply.cfm"
inurl:/wp-content/uploads/wp-backup-plus/
intitle:"index of /" authorized_keys
index of kcfinder/
index of /ckeditor
filetype:rdp default.rdp
filetype:txt "License Key"
intitle:"index of /" intext:/descargas/
intitle:"index of /" intext:/Download/
intext:"Powered by Abyss Web Server"
intitle:"index of" pagefile.sys
intitle:index of /.sql.gz intext:/backup/
inurl:/proc/tty/ index of
inurl:/sample/LvAppl/lvappl.htm
allinurl:control/multiview
allinurl:DialogHandler.aspx
intitle:"VertrigoServ" + "Welcome to VertrigoServ"
intitle:"Swagger UI - " + "Show/Hide"
inurl:/_vti_pvt/service.cnf | inurl:/_vti_inf.html | inurl:/_vti_bin/ | inurl:/_vti_bin/spsdisco.aspx
intitle: "Welcome to nginx!" + "Thank you for using nginx."
"vpnssl"
intext:jdbc:oracle filetype:java
intitle:" - Revision" + "subversion version"
Index of /.svn
inurl:"swagger-ui/index.html"
intitle:livezilla "Server Time"
intitle:"Sucuri WebSite Firewall - Access Denied"
intext:"Powered by phpSQLiteCMS" | intitle:"phpSQLiteCMS - A simple & lightweight CMS"
inurl:"/phpsqlitecms/cms/index.php"
intitle:"SQLiteManager" + intext:"Welcome to SQLiteManager version "
"This server is operated by OpenX."
intitle:"docker" intitle:"index of" config
inurl:wls-wsat intext:"weblogic.wsee.wstx.wsat"
intext:"Resource dumped by" intext:jcr -site:adobe.com
inurl:phpPgAdmin intext:"Cappuccino" | intext:"Blue/Green"
inurl:filebrowser.wcgp?subDir Communigate
ext:env intext:APP_ENV= | intext:APP_DEBUG= | intext:APP_KEY=
inurl:/Portal/Portal.mwsl?PriNav=FileBrowser
inurl:"/wp-json/" -wordpress
inurl:"/saml2?SAMLRequest="
inurl:home.tcl intitle:gaia
"[HKEY_CURRENT_USERSoftwareSimonTathamPuTTYSessions]" ext:reg
inurl:"/uddiexplorer/searchpublicregistries.jsp"
inurl="/uddiexplorer/SetupUDDIExplorer.jsp"
intitle:login "recruiter" | "employer" | "candidate"
filetype:reg reg HKEY_CURRENT_USER intext:password
inurl:department intext:"hardware inventory" firewall router ext:(doc | pdf | xls| psw | ppt | pps | xml | txt | ps | rtf | odt | sxw )
intext:"authentication" intranet password login inurl:account ext:(doc | pdf | xls| psw | ppt | pps | xml | txt | ps | rtf | odt | sxw | xlsx | docx | mail)
inurl:login intext:"reset your password"
intext:"Powered by Nesta"
Coldbox | contentbox | commandbox "Powered by ContentBox"
intext:(username | user | email | sign on | login | auth) admin dashboard | panel -stackoverflow
inurl:login.do? | shoplogin.do | adminlogin
intext:"Powered by Typesetter"
intext:"Powered by (Quantum | Quantum CMS | CMS)
inurl:"Default+Administrator+View"
inur:"arsys/forms" | "arsys/shared" | "/arsys/home"
filetype:txt $9$ JunOS
filetype:txt line vty 0 4
"ProQuest provides subscription access to numerous premium technical journals, dissertations and other information databases."
intext:"paytm" intitle:"index of"
intitle:"Log in - WhatsUp Gold"
intitle:"OAuth Server Login"
inurl:"standalone.xml" intext:"password>"
intext:Modified files in JOE when it aborted on JOE was aborted because the terminal closed
intext:"please find attached" "login" | password ext:pdf
intitle:Login inurl:login.php intext:admin/admin
intext:"KRAB-DECRYPT.txt" intitle:"index of"
intext:pure-ftpd.conf intitle:index of
intext:my.cnf intitle:index of
configuration> + filetype:config -github.com
inurl:logs/gravityforms
inurl:robots.txt intext:Disallow: /web.config
/_wpeprivate/config.json
intext:"Powered by Sentora" -github.com
inurl:"build.xml" intext:"tomcat.manager.password"
/var/www/manage/storage/logs/laravel- ext:log
site:drive.google.com /preview intext:movie inurl:flv | wmv | mp4 -pdf -edit -view
inurl:/yum.log | intitle:yum.log + ext:log
intitle:"index of" intext:twr.html
intitle:"index of" intext:login.csv
inurl:/banking.jsp?fldsegment=
inurl:/INALogin.jsp
intext:ZAP Scanning Report Summary of Alerts ext:html
inurl:"trello.com" and intext:"username" and intext:"password"
inurl:/typo3/typo3conf
inurl:/_hcms/
intext:"define('DB_NAME'," ext:txt
intext:"class JConfig {" inurl:configuration.php
intitle:backup+index of
inurl:/wp-json/wp/v2/users/ "id":1,"name":" -wordpress.stackexchange.com -stackoverflow.com
inurl:"wp-license.php?file=../..//wp-config"
intext:"M3R1C4 SHELL BACKDOOR"
intitle:"phpVirtualBox - VirtualBox Web Console"
intext:"PHP Version " ext:php intext:"disabled" intext:"Build Date" intext:"System" intext:"allow_url_fopen"
intext:"Build dashboard" intext:"Project" intext:"Plan" intext:"Build"
"index of" "database.sql.zip"
inurl:/wp-content/ai1wm-backups + wpress
ext:ppk ssh key -github.com -gitlab
inurl:conf/tomcat-users.xml -github
"index of" "database_log"
inurl:/usersignin?
inurl:"/gitweb.cgi?"
inurl:elmah.axd intext:"Powered by ELMAH" -inurl:detail
"index of" /wp-content/uploads/shell.php
"battlefield" "email" site:pastebin.com
"File Manager - Current disk free"
"Index of" "database.sql"
inurl:wp-config.bak
inurl: "Mister Spy" | intext:"Mister Spy & Souheyl Bypass Shell"
intext:"Thank you for using BIG-IP."
inurl:login.php.bak
intitle:"index of" ".travis.yml" | ".travis.xml"
intitle:"index of" "laravel.log" | "main.yaml" | "server.cfg"
"ansible.log" | "playbook.yaml" | ".ansible.cfg" | "playbook.yml" | host.ini intitle:"index of"
intext:"rabbit_password" | "service_password" filetype:conf
"whoops! there was an error." "db_password"
swiftmailer intitle:"index of" "smtp.yml" | "smtp.xml"
intitle:"index of" "config.yml" | "config.xml" intext:login | auth
intitle:"index of" "config.yml" | "config.xml" intext:login | auth
intitle:"index of" ".gitignore"
intext:APIKey ext:js | xml | yml | txt | conf | py -github -stackoverflow intitle:"index of"
inurl:tests/mocks intext:autoloader
inurl:lighttpd.conf lighttpd site:github.com
-site:smarty.net ext:tpl intext:"
inurl:nginx.conf nginx site:github.com
intext:"successfully" intitle:"index of" config | log | logged -stackoverflow
ext:log intext:"connection" intitle:"index of" -stackoverflow
employee "training" intitle:index.of ext:doc | pdf | xls |docx |xlsx
hardware | software "migration" intitle:index.of ext:xls | xlsx | doc | docx | pdf
"var miner=new CryptoLoot.Anonymous" intext:CryptoLoot.Anonymous
inurl:secure/dashboard jspa
inurl:travis.yml tornado site:github.com
intext:"login" department | admin | manager | company | host filetype:xls | xlsx -community -github
inurl:"/p3p.xml" | intitle: "p3p.xml" -github.com
inurl:"/tiny_mce/plugins/ajaxfilemanager/inc/data.php" | inurl:"/tiny_mce/plugins/ajaxfilemanager/ajax_create_folder.php" -github
intitle:index.of id_rsa -id_rsa.pub
intext:"please change your" password |code | login file:pdf | doc | txt | docx -github
"air confirmation" "passenger(s)"
intitle:HTTP Server Test Page powered by CentOS
inurl:"debug/default/view?panel=config"
inurl:configuration.php and intext:"var $password="
inurl:/dbcp.properties + filetype:properties -github.com
inurl:"root?originalDomain"
inurl:"/jira/login.jsp" intitle:"JIRA login"
intitle:"manager area" password -stackoverflow.com
"Copyright Metislab" password
filetype:txt Administrator:500:
nd=m_fundraising_detail "login here"
inurl:login.jsp intitle:"admin"
inurl:/wp-includes/certificates/
filetype:xls | xlsx intext:software license site:.gov
filetype:xls | xlsx intext:cisco -cisco.com site:.gov
intext:vmware virtual site:.gov filetype:xls | xlsx | doc | pdf
(intitle:"plexpy - home" OR "intitle:tautulli - home") AND intext:"libraries"
intext:define('AUTH_KEY', ' wp-config.php filetype:txt
"Powered by 2Moons"
intitle:"UltraDNS Client Redirection Service"
"Powered byPlanet eStream"
intitle:"This is pdfTeX, Version"
inurl:wp-config-backup.txt
"webkactus"
"CCCLogin.aspx"
"PaperCut Login"
intext:cv OR intext:curriculum vitae "passport details" ext:doc -template
intitle:"MyWebSQL" + "User ID: Password:"
intitle:"SSL VPN Service" + intext:"Your system administrator provided the following information to help understand and remedy the security conditions:"
intitle:"apache tomcat/" "Apache Tomcat examples"
filetype:png | "proportal"
frmLogin
"2004 - 2018 iboss, Inc. All rights reserved."
intitle:Wagtail.-.Sign in intext:Javascript.is.required.to.use.Wagtail
inurl:'/SSI/Auth/ip_configuration.htm'
intitle:"Malware Analysis Report"
intext:"Powered by www.yawcam.com"
allintitle:restricted filetype:doc site:gov
intext:"default values: admin/1234"
"password.xlsx" ext:xlsx
"username.xlsx" ext:xlsx
intitle:"index of /bins" arm
inurl:/admin intitle:Pulse.CMS -pulsecms.com
intext:Omeka*Username Powered.by.Omeka inurl:admin -github -omeka.org
filetype:gitattributes intext:CHANGELOG.md -site:github.com
inurl:/sitefinity intext:Copyright.(c)*Telerik. Site.Finity
"index of /ups.com/WebTracking"
filetype:env intext:REDIS_PASSWORD
filetype:env intext:AWS_SECRET
filetype:env intext:mail_host + intext:bluehost
intitle:'System Web Interface: WATTrouter M'
inurl:"/logon.aspx?ReturnUrl="
inurl:login.jsp?permissionViolation
intext:Connect.with.Finalsite intitle:admin -facebook
inurl:/contao/main ext:php -community -github
inurl:/CMSPages/logon ext:aspx
inurl:/index.php/login intext:Concrete.CMS
"Powered by Open Source Chat Platform Rocket.Chat."
inurl:'listprojects.spr'
inurl:'/blog/Account/login.aspx'
inurl:composer.json codeigniter -site:github.com
allintext:'HttpFileServer 2.3k'
intext:2001.-.2018.umbraco.org ext:aspx
AndroidManifest ext:xml -github -gitlab -googlesource
allintitle: "Flexi Press System"
intitle:"Netgear™ - NETGEAR Configuration Manager Login"
inurl:jpegpull.htm
inurl:"user_login/" bitcoin | crypto | wallet
inurl:"RootFolder=" Allitems "confidential" | "classified" | "passwords" | username
inurl:"AllItems.aspx?FolderCTID=" "firewall" | "proxy" | "configuration" | "account"
inurl:"q=user/password"
site:showmyhomework.co.uk/school/homeworks/ "password"
inurl:/munin/localdomain/localhost.localdomain/open_files.html
inurl:"?db_backup" | inurl:"dbbackup" -site:github.com "sql.gz" | "sql.tgz" | "sql.tar" | "sql.7z"
inurl:"paypal" intitle:"index of" backup | db | access -github
intitle:"index.of" inurl:"cvs" login | passwd | password | access | pass -github -pub
intitle:login laboratory | "nuclear" | physics "password" authentication
inurl:revslider inurl:'/revslider+port'
inurl:fisheye AND inurl:changelog -site:atlassian.com -site:github.com -intext:"Log in to FishEye"
inurl:"/wp-content/uploads/db-backup"
"Powered by Apache Subversion version"
intext:"this login can be used only once" inurl:user intitle:"reset password"
intitle:"Login" inurl:"/itim/self" | inurl:"/itim/ui" -ibm.com
filetype:doc inurl:"gov" intext:"default password is"
site:trello.com intext:mysql AND intext:password -site:developers.trello.com -site:help.trello.com
intitle:"Powered by Qualys SSL Labs"
intext:"PuTTY log" ext:log "password" -supportforums -github
intitle:"apache tomcat/" + "Find additional important configuration information in:"
intitle:"Index of" intext:"Login Data"
inurl:"/App.Config" + ext:config + "password=" -github -git
intitle:"Statistics Report for HAProxy" + "statistics report for pid"
"RDServer Product information" | inurl:"/rdagent.jsp"
ext:txt {"wallet_address" :", "pool_address" : " ", "pool_password" -git
intitle:"Apache2 Debian Default Page: It works"
intitle:Upload inurl:/cgi-bin/filechucker.cgi
inurl:..//drivers/etc/ intitle:index of
intitle:Munin :: overview
index of /node_modules/ -github -stackoverflow
inurl:"mjpg/video.cgi?resolution="
inurl:"/bigdump.php" + intitle:"BigDump ver."
inurl:?wp-commentsrss2.php -git
inurl:"servlet/ViewFormServlet?" "pwd"
intitle:"BMC Remedy Mid Tier" "login"
inurl:/.well-known/security.txt
inurl:/mailscanner/login.php
inurl:/daten/webyep-log.txt
inurl:rvsindex.php & /rvsindex.php?/user/login
intitle:"Open Source HRMS" intext:"powered by"
inurl:default.aspx?ReturnUrl=/spssmr -stackoverflow -youtube.com -github
inurl:"/SAMLLogin/" -github
inurl:"/user/register" "Powered by Drupal" -CAPTCHA -"Access denied"
intext:build:SVNTag= JBoss intitle:Administration Console inurl:web-console
Codeigniter filetype:sql intext:password | pwd intext:username | uname intext: Insert into users values
"login" "adp login" -adplogin.us -adplogin.org -adplogin.net
intitle:"index.of" | inurl:/filemanager/connectors/ intext:uploadtest.html
intitle:index.of inurl:/websendmail/
:DIR | intitle:index of inurl://whatsapp/
inurl:report.cgi?dashboard=
intitle:"index.of" "places.sqlite" "key3.db" -mozilla.org
intitle:"index.of" "places.sqlite" "Mail" thunderbird -mozilla.org -scan
inurl:"/Admin/Login?ReturnUrl=" -github.com -gitlab.com
filetype:config "" "password" "web.config" -stackoverflow -youtube.com -github
"login" inurl:"account/auth" -github -gitlab -stackoverflow
ext:ini Robust.ini filetype:ini "password"
ext:adr adr filetype:adr "bookmarks.adr"
inurl:":2083/login/?user="
intitle:index.of home/000~root~000/
intitle:"Index.Of.Applications (Parallels)" -stackoverflow -quora
inurl:"config.xml" "password" ext:xml -stackoverflow.com -github.com
inurl:"/forgotpwd.jspx"
inurl:"ssologin/" -github.com
inurl:"cmd=auth?" -github -stackoverflow -gitlab
inurl:"/initiatesso?providerid=" -github.com
"Oracle peoplesoft sign in" inurl:"cmd=login?" -github -stackoverflow -gitlab
inurl:"/Setup/Default.aspx" "mojoPortal"
inurl:"/startSSO.ping?" -stackoverflow.com
intitle:"Index Of" intext:".Trash"
inurl:"databases.yml" ext:yml password -github
intitle:"index.of.virtualbox" -mirror -mirrors -public -ubuntu.com -edu -pub
intext:"Powered by Nibbleblog"
inurl:/host.txt + filetype:txt + "password"
intitle:"Installing TYPO3 CMS"
intitle:"Index Of" intext:".vscode"
intext:"https://chat.whatsapp.com/invite/" intitle:"Your Search For Company/Subject/Whatever"
"Declassified and Approved for Release by" filetype: pdf
"login" intitle:"scada login"
intitle:"index of /" inanchor:.kdbx
intitle:"miniProxy"
site:pastebin.com "rcon_password"
intitle:"Index of /logs/" "lighttpd"
filetype:env intext:"APP_ENV"
filetype:log inurl:"log" "[SERVER_SOFTWARE]"
CakePHP inurl:database.php intext:db_password
ext:php + inurl:"ajaxfilemanager.php" + intext:"Current Folder Path"
CakePHP filetype:sql intext:password | pwd intext:username | uname intext: Insert into users values
intitle:"Deluge: Web UI 1.3"
intitle:"Deluge: Web UI" inurl:":8112"
intext:database inurl:"laravel.log" ext:log
intitle:"private login" username -github
dwsync.xml intitle:index of -gitlab -github
allinurl:mc4wp-debug.log ext:log
config.yaml intitle:"index of" vagrantfile
inurl:intranet/login login
intitle:"partners login"
inurl:"login.php?referer=profile.php"
intitle:"login credit" "login"
intitle:"login form" "powered by" -tutorial
"department" | "agency" | "government" "intitle:"login form" -youtube -template
"service" | "military" | "federal" "intitle:"login form" -youtube -template -stackoverflow
"login" "secure" "intitle:"online banking" -youtube -template -stackoverflow -stackexchange
intitle:"login" | intitle:"sign in" "member" "private" "admin" "club" -stackoverflow -github -youtube
intitle:"login" | intitle:"hospital" "patient" "clinic" "admin" "medical" "login" -stackoverflow -github -youtube
intext:"[***] Results from" + ext:txt + "snort-"
intitle:CV+index of
intitle:"Please login" "username" "password"
"username" "password" intitle:"login here"
inurl:"form_id" login username password
intitle:access your account" login
intitle:your access id is" login -youtube
intitle:Control Panel "Login with your username and password below." +"Email" +"Powered by"
inurl:"apps/backend/config/"
intext:password inurl:"/log/production" ext:log
intitle:"index of" inurl:"paypal" log
":: Arachni Web Application Security Report"
intitle:"Control Panel" + emailmarketer
intitle:"Axis Happiness Page" "Examining webapp configuration"
intitle:"index of" intext:"pip-selfcheck.json"
inurl:/?=PHPB8B5F2A0-3C92-11d3-A3A9-4C7B08C10000 | inurl:/?=PHPE9568F35-D428-11d2-A769-00AA001ACF42
intitle:"Proberv0." | inurl:/proberv.php
"var miner = new CoinHive" intext:document.domain
intitle:Login to CMS Made Simple + inurl:/cmsms
intitle:"index of" docker-compose.yml
intitle:"index of" .env
inurl:"/forms/frmservlet?config=" login
intitle:tm4web login | logon | account | member | password
filetype:sql intext:password | pass | passwd intext:username intext:INSERT INTO `users` VALUES
inurl:/gravity_forms/logs ext:txt
intext:"Dr.Web (R) Anti-virus. Virus base add-on" + ext:txt
intitle:"Yawcam" inurl:8081
ext:pem "PRIVATE KEY" -site:facebook.com -example -test*
inurl:control/camerainfo
"IBM Security AppScan Report" ext:pdf
inurl:"/etc/fail2ban/" + ext:conf
intext:"Powered by ViewVC" | intitle:"ViewVC Repository Listing"
inurl:cloud_main.asp
inurl:"server-status" "Server Version: Apache/" "Server Built: " "Server uptime:" "Total accesses" "CPU Usage:"
"database_password" filetype:yml "config/parameters.yml
inurl::5601/app/kibana
inurl:"index.php?option=com_joomanager"
"MAIL_PASSWORD" filetype:env
"database_password" filetype:yml "config/parameters.yml"
intitle:"netsparker scan report" ext:pdf
inurl:/fantastico_fileslist.txt + ext:txt
inurl:public "Powered by SecureW2"
inurl:/openwebmail/cgi-bin/openwebmail/etc/
allinurl:awstats.pl?config=
inurl:/install/stringnames.txt
intitle:"Burp Scanner Report" | "Report generated by Burp Scanner"
inurl:"plesk-stat"
inurl:"/xmlrpc.php?rsd" & ext:php
intitle: "Generated by Acunetix WVS Reporter"
inurl:/frontend/paper_lantern/index.html
allintitle:"Forum Post Assistant :" ext:php -site:joomla.org
"[LocalizedFileNames]" inurl:"desktop.ini" ext:ini -git -wiki
"[Tera Term]" inurl:"teraterm.ini" ext:ini -git
"ADS-B Receiver Live Dump1090 Map "
inurl:/add_vhost.php?lang=
inurl:"main.php?action=db"
inurl:module=coreHome
intitle:index.of intext:zc_install intitle:zen-cart
inurl:"/cgi-bin/filemanager/Manager.pl"
"Application Blocked!" "Google bot"
"Email delivery powered by Google" ext:pdf OR ext:txt
inurl:/login/index.php intitle:CentOS
intitle:"PHP Web Stat - Sysinfo" intext:php inurl:stat/sysinfo.php
"SiteBar Bookmark Manager" inurl:index.php?w=
inurl:"/jde/E1Menu.maf"
intitle:"Solr Admin" "Solr Query Syntax"
intitle:"Index Of" intext:sftp-config.json
inurl:"test/php/test.html" Plesk File
intitle:Armstrong Hot Water System Monitoring
inurl:embed.html inurl:dvr
inurl:"/libs/granite/core/content/login.html"
intitle:"Chorus 2 - Kodi web interface"
intitle:Kodi inurl:":8080" "Music. Music;"
intitle:"rutorrent v3" AND intext:Uploaded -github.com
ext:config + " password=" + "
intitle:"WAGO Ethernet web-based-management"
ext:jsp intext:"jspspy" intitle:"Jspspy web~shell V1.0"
intitle:"Nport web console"
inurl:"mgl-instagram-gallery/single-gallery.php?media"
"password" + ext:conf "Modem Type = USB Modem"
"lv_poweredBy"
```

## Dorks 2 <a name="_d2"></a>

```
"admin account info" filetype:log
!Host=*.* intext:enc_UserPassword=* ext:pcf
"# -FrontPage-" ext:pwd inurl:(service | authors | administrators | users) "# -FrontPage-" inurl:service.pwd
"AutoCreate=TRUE password=*"
"http://*:*@www" domainname
"index of/" "ws_ftp.ini" "parent directory"
"liveice configuration file" ext:cfg -site:sourceforge.net
"parent directory" +proftpdpasswd
Duclassified" -site:duware.com "DUware All Rights reserved"
duclassmate" -site:duware.com
Dudirectory" -site:duware.com
dudownload" -site:duware.com
Elite Forum Version *.*"
Link Department"
"sets mode: +k"
"your password is" filetype:log
DUpaypal" -site:duware.com
allinurl: admin mdb
auth_user_file.txt
config.php
eggdrop filetype:user user
enable password | secret "current configuration" -intext:the
etc (index.of)
ext:asa | ext:bak intext:uid intext:pwd -"uid..pwd" database | server | dsn
ext:inc "pwd=" "UID="
ext:ini eudora.ini
ext:ini Version=4.0.0.4 password
ext:passwd -intext:the -sample -example
ext:txt inurl:unattend.txt
ext:yml database inurl:config


filetype:bak createobject sa
filetype:bak inurl:"htaccess|passwd|shadow|htusers"
filetype:cfg mrtg "target
filetype:cfm "cfapplication name" password
filetype:conf oekakibbs
filetype:conf slapd.conf
filetype:config config intext:appSettings "User ID"
filetype:dat "password.dat"
filetype:dat inurl:Sites.dat
filetype:dat wand.dat
filetype:inc dbconn
filetype:inc intext:mysql_connect
filetype:inc mysql_connect OR mysql_pconnect
filetype:inf sysprep
filetype:ini inurl:"serv-u.ini"
filetype:ini inurl:flashFXP.ini
filetype:ini ServUDaemon
filetype:ini wcx_ftp
filetype:ini ws_ftp pwd
filetype:ldb admin
filetype:log "See `ipsec --copyright"
filetype:log inurl:"password.log"
filetype:mdb inurl:users.mdb
filetype:mdb wwforum
filetype:netrc password
filetype:pass pass intext:userid
filetype:pem intext:private
filetype:properties inurl:db intext:password
filetype:pwd service
filetype:pwl pwl
filetype:reg reg +intext:"defaultusername" +intext:"defaultpassword"
filetype:reg reg +intext:â? WINVNC3â?
filetype:reg reg HKEY_CURRENT_USER SSHHOSTKEYS
filetype:sql "insert into" (pass|passwd|password)
filetype:sql ("values * MD5" | "values * password" | "values * encrypt")
filetype:sql +"IDENTIFIED BY" -cvs
filetype:sql password
filetype:url +inurl:"ftp://" +inurl:";@"
filetype:xls username password email

htpasswd
htpasswd / htgroup
htpasswd / htpasswd.bak

intext:"enable password 7"
intext:"enable secret 5 $"
intext:"EZGuestbook"
intext:"Web Wiz Journal"

intitle:"index of" intext:connect.inc
intitle:"index of" intext:globals.inc
intitle:"Index of" passwords modified
intitle:"Index of" sc_serv.conf sc_serv content
intitle:"phpinfo()" +"mysql.default_password" +"Zend s?ri?ting Language Engine"
intitle:dupics inurl:(add.asp | default.asp | view.asp | voting.asp) -site:duware.com
intitle:index.of administrators.pwd
intitle:Index.of etc shadow
intitle:index.of intext:"secring.skr"|"secring.pgp"|"secring.bak"
intitle:rapidshare intext:login



inurl:"calendars?ri?t/users.txt"
inurl:"editor/list.asp" | inurl:"database_editor.asp" | inurl:"login.asa" "are set"
inurl:"GRC.DAT" intext:"password"
inurl:"Sites.dat"+"PASS="
inurl:"slapd.conf" intext:"credentials" -manpage -"Manual Page" -man: -sample
inurl:"slapd.conf" intext:"rootpw" -manpage -"Manual Page" -man: -sample
inurl:"wvdial.conf" intext:"password"
inurl:/db/main.mdb
inurl:/wwwboard
inurl:/yabb/Members/Admin.dat
inurl:ccbill filetype:log
inurl:cgi-bin inurl:calendar.cfg
inurl:chap-secrets -cvs
inurl:config.php dbuname dbpass
inurl:filezilla.xml -cvs
inurl:lilo.conf filetype:conf password -tatercounter2000 -bootpwd -man
inurl:nuke filetype:sql
inurl:ospfd.conf intext:password -sample -test -tutorial -download
inurl:pap-secrets -cvs
inurl:pass.dat
inurl:perform filetype:ini
inurl:perform.ini filetype:ini
inurl:secring ext:skr | ext:pgp | ext:bak
inurl:server.cfg rcon password
inurl:ventrilo_srv.ini adminpassword
inurl:vtund.conf intext:pass -cvs
inurl:zebra.conf intext:password -sample -test -tutorial -download

LeapFTP intitle:"index.of./" sites.ini modified
master.passwd
mysql history files
NickServ registration passwords
passlist
passlist.txt (a better way)
passwd
passwd / etc (reliable)
people.lst
psyBNC config files
pwd.db
server-dbs "intitle:index of"
signin filetype:url
spwd.db / passwd
trillian.ini
wwwboard WebAdmin inurl:passwd.txt wwwboard|webadmin
[WFClient] Password= filetype:ica
intitle:"remote assessment" OpenAanval Console
intitle:opengroupware.org "resistance is obsolete" "Report Bugs" "Username" "password"
"bp blog admin" intitle:login | intitle:admin -site:johnny.ihackstuff.com
"Emergisoft web applications are a part of our"
"Establishing a secure Integrated Lights Out session with" OR intitle:"Data Frame - Browser not HTTP 1.1 compatible" OR intitle:"HP Integrated Lights-
"HostingAccelerator" intitle:"login" +"Username" -"news" -demo
"iCONECT 4.1 :: Login"
"IMail Server Web Messaging" intitle:login
"inspanel" intitle:"login" -"cannot" "Login ID" -site:inspediumsoft.com
"intitle:3300 Integrated Communications Platform" inurl:main.htm
"Login - Sun Cobalt RaQ"
"login prompt" inurl:GM.cgi
"Login to Usermin" inurl:20000
"Microsoft CRM : Unsupported Browser Version"
"OPENSRS Domain Management" inurl:manage.cgi
"pcANYWHERE EXPRESS Java Client"
"Please authenticate yourself to get access to the management interface"
"please log in"
"Please login with admin pass" -"leak" -sourceforge



CuteNews" "2003..2005 CutePHP"
DWMail" password intitle:dwmail
Merak Mail Server Software" -.gov -.mil -.edu -site:merakmailserver.com
Midmart Messageboard" "Administrator Login"
Monster Top List" MTL numrange:200-
UebiMiau" -site:sourceforge.net
"site info for" "Enter Admin Password"
"SquirrelMail version" "By the SquirrelMail development Team"
"SysCP - login"
"This is a restricted Access Server" "Javas?ri?t Not Enabled!"|"Messenger Express" -edu -ac
"This section is for Administrators only. If you are an administrator then please"
"ttawlogin.cgi/?action="
"VHCS Pro ver" -demo
"VNC Desktop" inurl:5800
"Web-Based Management" "Please input password to login" -inurl:johnny.ihackstuff.com
"WebExplorer Server - Login" "Welcome to WebExplorer Server"
"WebSTAR Mail - Please Log In"
"You have requested access to a restricted area of our website. Please authenticate yourself to continue."
"You have requested to access the management functions" -.edu


(intitle:"Please login - Forums
UBB.threads")|(inurl:login.php "ubb")
(intitle:"Please login - Forums
WWWThreads")|(inurl:"wwwthreads/login.php")|(inurl:"wwwthreads/login.pl?Cat=")
(intitle:"rymo Login")|(intext:"Welcome to rymo") -family
(intitle:"WmSC e-Cart Administration")|(intitle:"WebMyStyle e-Cart Administration")
(inurl:"ars/cgi-bin/arweb?O=0" | inurl:arweb.jsp) -site:remedy.com -site:mil
4images Administration Control Panel
allintitle:"Welcome to the Cyclades"
allinurl:"exchange/logon.asp"
allinurl:wps/portal/ login
ASP.login_aspx "ASP.NET_SessionId"
CGI:IRC Login
ext:cgi intitle:"control panel" "enter your owner password to continue!"
ez Publish administration
filetype:php inurl:"webeditor.php"
filetype:pl "Download: SuSE Linux Openexchange Server CA"
filetype:r2w r2w
intext:""BiTBOARD v2.0" BiTSHiFTERS Bulletin Board"
intext:"Fill out the form below completely to change your password and user name. If new username is left blank, your old one will be assumed." -edu


intext:"Mail admins login here to administrate your domain."
intext:"Master Account" "Domain Name" "Password" inurl:/cgi-bin/qmailadmin
intext:"Master Account" "Domain Name" "Password" inurl:/cgi-bin/qmailadmin
intext:"Storage Management Server for" intitle:"Server Administration"
intext:"Welcome to" inurl:"cp" intitle:"H-SPHERE" inurl:"begin.html" -Fee
intext:"vbulletin" inurl:admincp


intitle:"*- HP WBEM Login" | "You are being prompted to provide login account information for *" | "Please provide the information requested and press
intitle:"Admin Login" "admin login" "blogware"
intitle:"Admin login" "Web Site Administration" "Copyright"
intitle:"AlternC Desktop"
intitle:"Athens Authentication Point"
intitle:"b2evo > Login form" "Login form. You must log in! You will have to accept cookies in order to log in" -demo -site:b2evolution.net
intitle:"Cisco CallManager User Options Log On" "Please enter your User ID and Password in the spaces provided below and click the Log On button to co
intitle:"ColdFusion Administrator Login"
intitle:"communigate pro * *" intitle:"entrance"
intitle:"Content Management System" "user name"|"password"|"admin" "Microsoft IE 5.5" -mambo
intitle:"Content Management System" "user name"|"password"|"admin" "Microsoft IE 5.5" -mambo
intitle:"Dell Remote Access Controller"
intitle:"Docutek ERes - Admin Login" -edu
intitle:"Employee Intranet Login"
intitle:"eMule *" intitle:"- Web Control Panel" intext:"Web Control Panel" "Enter your password here."
intitle:"ePowerSwitch Login"
intitle:"eXist Database Administration" -demo
intitle:"EXTRANET * - Identification"
intitle:"EXTRANET login" -.edu -.mil -.gov
intitle:"EZPartner" -netpond
intitle:"Flash Operator Panel" -ext:php -wiki -cms -inurl:asternic -inurl:sip -intitle:ANNOUNCE -inurl:lists
intitle:"i-secure v1.1" -edu
intitle:"Icecast Administration Admin Page"
intitle:"iDevAffiliate - admin" -demo
intitle:"ISPMan : Unauthorized Access prohibited"
intitle:"ITS System Information" "Please log on to the SAP System"
intitle:"Kurant Corporation StoreSense" filetype:bok
intitle:"ListMail Login" admin -demo
intitle:"Login -


Easy File Sharing Web Server"
intitle:"Login Forum
AnyBoard" intitle:"If you are a new user:" intext:"Forum
AnyBoard" inurl:gochat -edu
intitle:"Login to @Mail" (ext:pl | inurl:"index") -dwaffleman
intitle:"Login to Cacti"
intitle:"Login to the forums - @www.aimoo.com" inurl:login.cfm?id=
intitle:"MailMan Login"
intitle:"Member Login" "NOTE: Your browser must have cookies enabled in order to log into the site." ext:php OR ext:cgi
intitle:"Merak Mail Server Web Administration" -ihackstuff.com
intitle:"microsoft certificate services" inurl:certsrv
intitle:"MikroTik RouterOS Managing Webpage"
intitle:"MX Control Console" "If you can't remember"
intitle:"Novell Web Services" "GroupWise" -inurl:"doc/11924" -.mil -.edu -.gov -filetype:pdf
intitle:"Novell Web Services" intext:"Select a service and a language."
intitle:"oMail-admin Administration - Login" -inurl:omnis.ch
intitle:"OnLine Recruitment Program - Login"
intitle:"Philex 0.2*" -s?ri?t -site:freelists.org
intitle:"PHP Advanced Transfer" inurl:"login.php"
intitle:"php icalendar administration" -site:sourceforge.net
intitle:"php icalendar administration" -site:sourceforge.net
intitle:"phpPgAdmin - Login" Language
intitle:"PHProjekt - login" login password
intitle:"please login" "your password is *"
intitle:"Remote Desktop Web Connection" inurl:tsweb
intitle:"SFXAdmin - sfx_global" | intitle:"SFXAdmin - sfx_local" | intitle:"SFXAdmin - sfx_test"
intitle:"SHOUTcast Administrator" inurl:admin.cgi
intitle:"site administration: please log in" "site designed by emarketsouth"
intitle:"Supero Doctor III" -inurl:supermicro
intitle:"SuSE Linux Openexchange Server" "Please activate Javas?ri?t!"
intitle:"teamspeak server-administration
intitle:"Tomcat Server Administration"
intitle:"TOPdesk ApplicationServer"
intitle:"TUTOS Login"
intitle:"TWIG Login"
intitle:"vhost" intext:"vHost . 2000-2004"
intitle:"Virtual Server Administration System"
intitle:"VisNetic WebMail" inurl:"/mail/"
intitle:"VitalQIP IP Management System"
intitle:"VMware Management Interface:" inurl:"vmware/en/"
intitle:"VNC viewer for Java"
intitle:"web-cyradm"|"by Luc de Louw" "This is only for authorized users" -tar.gz -site:web-cyradm.org
intitle:"WebLogic Server" intitle:"Console Login" inurl:console
intitle:"Welcome Site/User Administrator" "Please select the language" -demos
intitle:"Welcome to Mailtraq WebMail"
intitle:"welcome to netware *" -site:novell.com
intitle:"WorldClient" intext:"? (2003|2004) Alt-N Technologies."
intitle:"xams 0.0.0..15 - Login"
intitle:"XcAuctionLite" | "DRIVEN BY XCENT" Lite inurl:admin
intitle:"XMail Web Administration Interface" intext:Login intext:password
intitle:"Zope Help System" inurl:HelpSys
intitle:"ZyXEL Prestige Router" "Enter password"
intitle:"inc. vpn 3000 concentrator"
intitle:("TrackerCam Live Video")|("TrackerCam Application Login")|("Trackercam Remote") -trackercam.com
intitle:asterisk.management.portal web-access
intitle:endymion.sak?.mail.login.page | inurl:sake.servlet
intitle:Group-Office "Enter your username and password to login"
intitle:ilohamail "


IlohaMail"
intitle:ilohamail intext:"Version 0.8.10" "
IlohaMail"
intitle:IMP inurl:imp/index.php3
intitle:Login * Webmailer
intitle:Login intext:"RT is ? Copyright"
intitle:Node.List Win32.Version.3.11
intitle:Novell intitle:WebAccess "Copyright *-* Novell, Inc"
intitle:open-xchange inurl:login.pl
intitle:Ovislink inurl:private/login
intitle:phpnews.login
intitle:plesk inurl:login.php3
inurl:"/admin/configuration. php?" Mystore
inurl:"/slxweb.dll/external?name=(custportal|webticketcust)"
inurl:"1220/parse_xml.cgi?"
inurl:"631/admin" (inurl:"op=*") | (intitle:CUPS)
inurl:":10000" intext:webmin
inurl:"Activex/default.htm" "Demo"
inurl:"calendar.asp?action=login"
inurl:"default/login.php" intitle:"kerio"
inurl:"gs/adminlogin.aspx"
inurl:"php121login.php"
inurl:"suse/login.pl"
inurl:"typo3/index.php?u=" -demo
inurl:"usysinfo?login=true"
inurl:"utilities/TreeView.asp"
inurl:"vsadmin/login" | inurl:"vsadmin/admin" inurl:.php|.asp

Code:

nurl:/admin/login.asp
inurl:/cgi-bin/sqwebmail?noframes=1
inurl:/Citrix/Nfuse17/
inurl:/dana-na/auth/welcome.html
inurl:/eprise/
inurl:/Merchant2/admin.mv | inurl:/Merchant2/admin.mvc | intitle:"Miva Merchant Administration Login" -inurl:cheap-malboro.net
inurl:/modcp/ intext:Moderator+vBulletin
inurl:/SUSAdmin intitle:"Microsoft Software upd?t? Services"
inurl:/webedit.* intext:WebEdit Professional -html
inurl:1810 "Oracle Enterprise Manager"
inurl:2000 intitle:RemotelyAnywhere -site:realvnc.com
inurl::2082/frontend -demo
inurl:administrator "welcome to mambo"
inurl:bin.welcome.sh | inurl:bin.welcome.bat | intitle:eHealth.5.0
inurl:cgi-bin/ultimatebb.cgi?ubb=login
inurl:Citrix/MetaFrame/default/default.aspx
inurl:confixx inurl:login|anmeldung
inurl:coranto.cgi intitle:Login (Authorized Users Only)
inurl:csCreatePro.cgi
inurl:default.asp intitle:"WebCommander"
inurl:exchweb/bin/auth/owalogon.asp
inurl:gnatsweb.pl
inurl:ids5web
inurl:irc filetype:cgi cgi:irc
inurl:login filetype:swf swf
inurl:login.asp
inurl:login.cfm
inurl:login.php "SquirrelMail version"
inurl:metaframexp/default/login.asp | intitle:"Metaframe XP Login"
inurl:mewebmail
inurl:names.nsf?opendatabase
inurl:ocw_login_username
inurl:orasso.wwsso_app_admin.ls_login
inurl:postfixadmin intitle:"postfix admin" ext:php
inurl:search/admin.php
inurl:textpattern/index.php
inurl:WCP_USER
inurl:webmail./index.pl "Interface"
inurl:webvpn.html "login" "Please enter your"
Login ("
Jetbox One CMS â?¢" | "
Jetstream ? *")
Novell NetWare intext:"netware management portal version"
Outlook Web Access (a better way)
PhotoPost PHP Upload
PHPhotoalbum Statistics
PHPhotoalbum Upload
phpWebMail
Please enter a valid password! inurl:polladmin

INDEXU
Ultima Online loginservers
W-Nailer Upload Area
intitle:"DocuShare" inurl:"docushare/dsweb/" -faq -gov -edu
"#mysql dump" filetype:sql
"#mysql dump" filetype:sql 21232f297a57a5a743894a0e4a801fc3
"allow_call_time_pass_reference" "PATH_INFO"
"Certificate Practice Statement" inurl:(PDF | DOC)
"Generated by phpSystem"
"generated by wwwstat"
"Host Vulnerability Summary Report"
"HTTP_FROM=googlebot" googlebot.com "Server_Software="
"Index of" / "chat/logs"
"Installed Objects Scanner" inurl:default.asp
"MacHTTP" filetype:log inurl:machttp.log
"Mecury Version" "Infastructure Group"
"Microsoft (R) Windows * (TM) Version * DrWtsn32 Copyright (C)" ext:log
"Most Submitted Forms and s?ri?ts" "this section"
"Network Vulnerability Assessment Report"
"not for distribution" confidential
"not for public release" -.edu -.gov -.mil
"phone * * *" "address *" "e-mail" intitle:"curriculum vitae"
"phpMyAdmin" "running on" inurl:"main.php"
"produced by getstats"
"Request Details" "Control Tree" "Server Variables"
"robots.txt" "Disallow:" filetype:txt
"Running in Child mode"
"sets mode: +p"
"sets mode: +s"
"Thank you for your order" +receipt
"This is a Shareaza Node"
"This report was generated by WebLog"
( filetype:mail | filetype:eml | filetype:mbox | filetype:mbx ) intext:password|subject
(intitle:"PRTG Traffic Grapher" inurl:"allsensors")|(intitle:"PRTG Traffic Grapher - Monitoring Results")
(intitle:WebStatistica inurl:main.php) | (intitle:"WebSTATISTICA server") -inurl:statsoft -inurl:statsoftsa -inurl:statsoftinc.com -edu -software -rob
(inurl:"robot.txt" | inurl:"robots.txt" ) intext:disallow filetype:txt
+":8080" +":3128" +":80" filetype:txt
+"HSTSNR" -"netop.com"
-site:php.net -"The PHP Group" inurl:source inurl:url ext:pHp
94FBR "ADOBE PHOTOSHOP"
AIM buddy lists
allinurl:/examples/jsp/snp/snoop.jsp
allinurl:cdkey.txt
allinurl:servlet/SnoopServlet
cgiirc.conf
cgiirc.conf
contacts ext:wml
data filetype:mdb -site:gov -site:mil

exported email addresses
ext:(doc | pdf | xls | txt | ps | rtf | odt | sxw | psw | ppt | pps | xml) (intext:confidential salary | intext:"budget approved") inurl:confidential
ext:asp inurl:pathto.asp
ext:ccm ccm -catacomb
ext:CDX CDX
ext:cgi inurl:editcgi.cgi inurl:file=
ext:conf inurl:rsyncd.conf -cvs -man
ext:conf NoCatAuth -cvs
ext:dat bpk.dat
ext:gho gho
ext:ics ics
ext:ini intext:env.ini
ext:jbf jbf
ext:ldif ldif
ext:log "Software: Microsoft Internet Information Services *.*"
ext:mdb inurl:*.mdb inurl:fpdb shop.mdb
ext:nsf nsf -gov -mil
ext:plist filetype:plist inurl:bookmarks.plist
ext:pqi pqi -database
ext:reg "username=*" putty
ext:txt "Final encryption key"
ext:txt inurl:dxdiag
ext:vmdk vmdk
ext:vmx vmx


filetype:asp DBQ=" * Server.MapPath("*.mdb")
filetype:bkf bkf
filetype:blt "buddylist"
filetype:blt blt +intext:screenname
filetype:cfg auto_inst.cfg
filetype:cnf inurl:_vti_pvt access.cnf
filetype:conf inurl:firewall -intitle:cvs
filetype:config web.config -CVS
filetype:ctt Contact
filetype:ctt ctt messenger
filetype:eml eml +intext:"Subject" +intext:"From" +intext:"To"
filetype:fp3 fp3
filetype:fp5 fp5 -site:gov -site:mil -"cvs log"
filetype:fp7 fp7
filetype:inf inurl:capolicy.inf
filetype:lic lic intext:key
filetype:log access.log -CVS
filetype:log cron.log
filetype:mbx mbx intext:Subject
filetype:myd myd -CVS
filetype:ns1 ns1
filetype:ora ora
filetype:ora tnsnames
filetype:pdb pdb backup (Pilot | Pluckerdb)
filetype:php inurl:index inurl:phpicalendar -site:sourceforge.net
filetype:pot inurl:john.pot
filetype:PS ps
filetype:pst inurl:"outlook.pst"
filetype:pst pst -from -to -date
filetype:qbb qbb
filetype:QBW qbw
filetype:rdp rdp
filetype:reg "Terminal Server Client"
filetype:vcs vcs
filetype:wab wab
filetype:xls -site:gov inurl:contact
filetype:xls inurl:"email.xls"
Financial spreadsheets: finance.xls
Financial spreadsheets: finances.xls
Ganglia Cluster Reports
haccess.ctl (one way)
haccess.ctl (VERY reliable)
ICQ chat logs, please...
intext:"Session Start * * * *:*:* *" filetype:log
intext:"Tobias Oetiker" "traffic analysis"
intext:(password | passcode) intext:(username | userid | user) filetype:csv
intext:gmail invite intext:http://gmail.google.com/gmail/a
intext:SQLiteManager inurl:main.php
intext:ViewCVS inurl:Settings.php
intitle:"admin panel" +"


RedKernel"
intitle:"Apache::Status" (inurl:server-status | inurl:status.html | inurl:apache.html)
intitle:"AppServ Open Project" -site:www.appservnetwork.com
intitle:"ASP Stats Generator *.*" "ASP Stats Generator" "2003-2004 weppos"
intitle:"Big Sister" +"OK Attention Trouble"
intitle:"curriculum vitae" filetype:doc
intitle:"edna:streaming mp3 server" -forums
intitle:"FTP root at"
intitle:"index of" +myd size
intitle:"Index Of" -inurl:maillog maillog size
intitle:"Index Of" cookies.txt size
intitle:"index of" mysql.conf OR mysql_config
intitle:"Index of" upload size parent directory
intitle:"index.of *" admin news.asp configview.asp
intitle:"index.of" .diz .nfo last modified
intitle:"Joomla - Web Installer"
intitle:"LOGREP - Log file reporting system" -site:itefix.no
intitle:"Multimon UPS status page"
intitle:"PHP Advanced Transfer" (inurl:index.php | inurl:showrecent.php )
intitle:"PhpMyExplorer" inurl:"index.php" -cvs
intitle:"statistics of" "advanced web statistics"
intitle:"System Statistics" +"System and Network Information Center"
intitle:"urchin (5|3|admin)" ext:cgi
intitle:"Usage Statistics for" "Generated by Webalizer"
intitle:"wbem" compaq login "Compaq Information Technologies Group"
intitle:"Web Server Statistics for ****"
intitle:"web server status" SSH Telnet
intitle:"Welcome to F-Secure Policy Manager Server Welcome Page"
intitle:"welcome.to.squeezebox"
intitle:admin intitle:login
intitle:Bookmarks inurl:bookmarks.html "Bookmarks
intitle:index.of "Apache" "server at"
intitle:index.of cleanup.log
intitle:index.of dead.letter
intitle:index.of inbox
intitle:index.of inbox dbx
intitle:index.of ws_ftp.ini
intitle:intranet inurl:intranet +intext:"phone"


inurl:"/axs/ax-admin.pl" -s?ri?t
inurl:"/cricket/grapher.cgi"
inurl:"bookmark.htm"
inurl:"cacti" +inurl:"graph_view.php" +"Settings Tree View" -cvs -RPM
inurl:"newsletter/admin/"
inurl:"newsletter/admin/" intitle:"newsletter admin"
inurl:"putty.reg"
inurl:"smb.conf" intext:"workgroup" filetype:conf conf
inurl:*db filetype:mdb
inurl:/cgi-bin/pass.txt
inurl:/_layouts/settings
inurl:admin filetype:xls
inurl:admin intitle:login
inurl:backup filetype:mdb
inurl:build.err
inurl:cgi-bin/printenv
inurl:cgi-bin/testcgi.exe "Please distribute TestCGI"
inurl:changepassword.asp
inurl:ds.py
inurl:email filetype:mdb
inurl:fcgi-bin/echo
inurl:forum filetype:mdb
inurl:forward filetype:forward -cvs
inurl:getmsg.html intitle:hotmail
inurl:log.nsf -gov
inurl:main.php phpMyAdmin
inurl:main.php Welcome to phpMyAdmin
inurl:netscape.hst
inurl:netscape.hst
inurl:netscape.ini
inurl:odbc.ini ext:ini -cvs
inurl:perl/printenv
inurl:php.ini filetype:ini
inurl:preferences.ini "[emule]"
inurl:profiles filetype:mdb
inurl:report "EVEREST Home Edition "
inurl:server-info "Apache Server Information"
inurl:server-status "apache"
inurl:snitz_forums_2000.mdb
inurl:ssl.conf filetype:conf
inurl:tdbin
inurl:vbstats.php "page generated"
inurl:wp-mail.php + "There doesn't seem to be any new mail."
inurl:XcCDONTS.asp
ipsec.conf
ipsec.secrets
ipsec.secrets
Lotus Domino address books
mail filetype:csv -site:gov intext:name
Microsoft Money Data Files
mt-db-pass.cgi files
MySQL tabledata dumps
mystuff.xml - Trillian data files
OWA Public Folders (direct view)
Peoples MSN contact lists
php-addressbook "This is the addressbook for *" -warning
phpinfo()
phpMyAdmin dumps
phpMyAdmin dumps
private key files (.csr)
private key files (.key)
Quicken data files
rdbqds -site:.edu -site:.mil -site:.gov


robots.txt
site:edu admin grades
site:www.mailinator.com inurl:ShowMail.do
SQL data dumps
Squid cache server reports
Unreal IRCd
WebLog Referrers
Welcome to ntop!
Fichier contenant des informations sur le r?seau :
filetype:log intext:"ConnectionManager2"
"apricot - admin" 00h
"by Reimar Hoven. All Rights Reserved. Disclaimer" | inurl:"log/logdb.dta"
"Network Host Assessment Report" "Internet Scanner"
"Output produced by SysWatch *"
"Phorum Admin" "Database Connection" inurl:forum inurl:admin
phpOpenTracker" Statistics
"powered | performed by Beyond Security's Automated Scanning" -kazaa -example
"Shadow Security Scanner performed a vulnerability assessment"
"SnortSnarf alert page"
"The following report contains confidential information" vulnerability -search
"The statistics were last upd?t?d" "Daily"-microsoft.com
"this proxy is working fine!" "enter *" "URL***" * visit
"This report lists" "identified by Internet Scanner"
"Traffic Analysis for" "RMON Port * on unit *"
"Version Info" "Boot Version" "Internet Settings"
((inurl:ifgraph "Page generated at") OR ("This page was built using ifgraph"))
Analysis Console for Incident Databases
ext:cfg radius.cfg
ext:cgi intext:"nrg-" " This web page was created on "


filetype:pdf "Assessment Report" nessus
filetype:php inurl:ipinfo.php "Distributed Intrusion Detection System"
filetype:php inurl:nqt intext:"Network Query Tool"
filetype:vsd vsd network -samples -examples
intext:"Welcome to the Web V.Networks" intitle:"V.Networks [Top]" -filetype:htm
intitle:"ADSL Configuration page"
intitle:"Azureus : Java BitTorrent Client Tracker"
intitle:"Belarc Advisor Current Profile" intext:"Click here for Belarc's PC Management products, for large and small companies."
intitle:"BNBT Tracker Info"
intitle:"Microsoft Site Server Analysis"
intitle:"Nessus Scan Report" "This file was generated by Nessus"
intitle:"PHPBTTracker Statistics" | intitle:"PHPBT Tracker Statistics"
intitle:"Retina Report" "CONFIDENTIAL INFORMATION"
intitle:"start.managing.the.device" remote pbx acc
intitle:"sysinfo * " intext:"Generated by Sysinfo * written by The Gamblers."
intitle:"twiki" inurl:"TWikiUsers"
inurl:"/catalog.nsf" intitle:catalog
inurl:"install/install.php"
inurl:"map.asp?" intitle:"WhatsUp Gold"
inurl:"NmConsole/Login.asp" | intitle:"Login - Ipswitch WhatsUp Professional 2005" | intext:"Ipswitch WhatsUp Professional 2005 (SP1)" "Ipswitch, Inc"


inurl:"sitescope.html" intitle:"sitescope" intext:"refresh" -demo
inurl:/adm-cfgedit.php
inurl:/cgi-bin/finger? "In real life"
inurl:/cgi-bin/finger? Enter (account|host|user|username)
inurl:/counter/index.php intitle:"+PHPCounter 7.*"
inurl:CrazyWWWBoard.cgi intext:"detailed debugging information"
inurl:login.jsp.bak
inurl:ovcgi/jovw
inurl:phpSysInfo/ "created by phpsysinfo"
inurl:portscan.php "from Port"|"Port Range"
inurl:proxy | inurl:wpad ext:pac | ext:dat findproxyforurl
inurl:statrep.nsf -gov
inurl:status.cgi?host=all
inurl:testcgi xitami
inurl:webalizer filetype:png -.gov -.edu -.mil -opendarwin
inurl:webutil.pl
Looking Glass
site:netcraft.com intitle:That.Site.Running Apache
"A syntax error has occurred" filetype:ihtml
"access denied for user" "using password"
"An illegal character has been found in the statement" -"previous message"
"ASP.NET_SessionId" "data source="
"Can't connect to local" intitle:warning
"Chatologica MetaSearch" "stack tracking"
"detected an internal error [IBM][CLI Driver][DB2/6000]"
"error found handling the request" cocoon filetype:xml
"Fatal error: Call to undefined function" -reply -the -next
"Incorrect syntax near"
"Incorrect syntax near"
"Internal Server Error" "server at"
"Invision Power Board Database Error"
"ORA-00933: SQL command not properly ended"
"ORA-12541: TNS:no listener" intitle:"error occurred"
"Parse error: parse error, unexpected T_VARIABLE" "on line" filetype:php
"PostgreSQL query failed: ERROR: parser: parse error"
"Supplied argument is not a valid MySQL result resource"
"Syntax error in query expression " -the
"The s?ri?t whose uid is " "is not allowed to access"
"There seems to have been a problem with the" " Please try again by clicking the Refresh button in your web browser."
"Unable to jump to row" "on MySQL result index" "on line"
"Unclosed quotation mark before the character string"
"Warning: Bad arguments to (join|implode) () in" "on line" -help -forum
"Warning: Cannot modify header information - headers already sent"
"Warning: Division by zero in" "on line" -forum



"Warning: mysql_connect(): Access denied for user: '*@*" "on line" -help -forum
"Warning: mysql_query()" "invalid query"
"Warning: pg_connect(): Unable to connect to PostgreSQL server: FATAL"
"Warning: Supplied argument is not a valid File-Handle resource in"
"Warning:" "failed to open stream: HTTP request failed" "on line"
"Warning:" "SAFE MODE Restriction in effect." "The s?ri?t whose uid is" "is not allowed to access owned by uid 0 in" "on line"
"SQL Server Driver][SQL Server]Line 1: Incorrect syntax near"
An unexpected token "END-OF-STATEMENT" was found
Coldfusion Error Pages
filetype:asp + "[ODBC SQL"
filetype:asp "Custom Error Message" Category Source
filetype:log "PHP Parse error" | "PHP Warning" | "PHP Error"
filetype:php inurl:"logging.php" "Discuz" error
ht://Dig htsearch error
IIS 4.0 error messages
IIS web server error messages
Internal Server Error
intext:"Error Message : Error loading required libraries."
intext:"Warning: Failed opening" "on line" "include_path"
intitle:"Apache Tomcat" "Error Report"
intitle:"Default PLESK Page"
intitle:"Error Occurred While Processing Request" +WHERE (SELECT|INSERT) filetype:cfm
intitle:"Error Occurred" "The error occurred in" filetype:cfm
intitle:"Error using Hypernews" "Server Software"
intitle:"Execution of this s?ri?t not permitted"
intitle:"Under construction" "does not currently have"
intitle:Configuration.File inurl:softcart.exe
MYSQL error message: supplied argument....
mysql error with query
Netscape Application Server Error page
ORA-00921: unexpected end of SQL command
ORA-00921: unexpected end of SQL command
ORA-00936: missing expression


PHP application warnings failing "include_path"
sitebuildercontent
sitebuilderfiles
sitebuilderpictures
Snitz! forums db path error
SQL syntax error
Supplied argument is not a valid PostgreSQL result
warning "error on line" php sablotron
Windows 2000 web server error messages
"ftp://" "www.eastgame.net"
"html allowed" guestbook
: vBulletin Version 1.1.5"
"Select a database to view" intitle:"filemaker pro"
"set up the administrator user" inurl:pivot
"There are no Administrators Accounts" inurl:admin.php -mysql_fetch_row
"Welcome to Administration" "General" "Local Domains" "SMTP Authentication" inurl:admin
"Welcome to Intranet"
"Welcome to PHP-Nuke" congratulations
"Welcome to the Prestige Web-Based Configurator"
"YaBB SE Dev Team"
"you can now password" | "this is a special page only seen by you. your profile visitors" inurl:imchaos
("Indexed.By"|"Monitored.By") hAcxFtpScan
(inurl:/shop.cgi/page=) | (inurl:/shop.pl/page=)
allinurl:"index.php" "site=sglinks"
allinurl:install/install.php
allinurl:intranet admin
filetype:cgi inurl:"fileman.cgi"
filetype:cgi inurl:"Web_Store.cgi"
filetype:php inurl:vAuthenticate
filetype:pl intitle:"Ultraboard Setup"
Gallery in configuration mode
Hassan Consulting's Shopping Cart Version 1.18
intext:"Warning: * am able * write ** configuration file" "includes/configure.php" -
intitle:"Gateway Configuration Menu"
intitle:"Horde :: My Portal" -"[Tickets"
intitle:"Mail Server CMailServer Webmail" "5.2"
intitle:"MvBlog powered"
intitle:"Remote Desktop Web Connection"
intitle:"Samba Web Administration Tool" intext:"Help Workgroup"
intitle:"Terminal Services Web Connection"
intitle:"Uploader - Uploader v6" -pixloads.com
intitle:osCommerce inurl:admin intext:"redistributable under the GNU" intext:"Online Catalog" -demo -site:oscommerce.com
intitle:phpMyAdmin "Welcome to phpMyAdmin ***" "running on * as root@*"


intitle:phpMyAdmin "Welcome to phpMyAdmin ***" "running on * as root@*"
inurl:"/NSearch/AdminServlet"
inurl:"index.php? module=ew_filemanager"
inurl:aol*/_do/rss_popup?blogID=
inurl:footer.inc.php
inurl:info.inc.php
inurl:ManyServers.htm
inurl:newsdesk.cgi? inurl:"t="
inurl:pls/admin_/gateway.htm
inurl:rpSys.html
inurl:search.php vbulletin
inurl:servlet/webacc
natterchat inurl:home.asp -site:natterchat.co.uk
XOOPS Custom Installation
inurl:htpasswd filetype:htpasswd
inurl:yapboz_detay.asp + View Webcam User Accessing
allinurl:control/multiview
inurl:"ViewerFrame?Mode="
intitle:"WJ-NT104 Main Page"
inurl:netw_tcp.shtml
intitle:"supervisioncam protocol"
```
