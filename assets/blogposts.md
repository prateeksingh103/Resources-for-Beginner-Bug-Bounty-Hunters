# Resources-for-Beginner-Bug-Bounty-Hunters

## Blog posts & Disclosed Reports 📝
A collection of Blog Posts ordered by Vulnerability Types
- [Starting out & Tips](#Starting-Out-&-Questions)
- [XSS](#XSS)
    - [DOM XSS](#DOM-XSS)
    - [Stored XSS](#Stored-XSS)
- [SSRF](#SSRF)
- [Vulnerability Scanning](#Vulnerability-Scanning)
- [Token / Authentication](#Token-/-Authentication)
- [SQL Injection](#SQL-Injection)
- [Mobile](#Mobile)
    - [iOS](#iOS)
    - [Android](#Android)
- [HTTP Desync](#HTTP-Desync)
- [File Upload](#File-Upload)
- [Automation](#Automation)
- [Buffer Overflow](#Buffer-Overflow)
- [IDOR](#IDOR)
- [GraphQL](#GraphQL)
- [RCE](#RCE)
- [Recon](#Recon)
- [Smart Contracts](#Smart-Contracts)
- [API](#API)
- [Misc](#Misc)
---
## Starting out & Tips
- [Basic Bug Bounty FAQ](http://blog.oath.ninja/basic-bug-bounty-faq/) - by [@thedawgyg](https://twitter.com/thedawgyg)
- [Getting started in Cyber Security in 2019 – The Complete Guide](https://www.ceos3c.com/hacking/getting-started-cyber-security-complete-guide/) - by ceos3c
- [WTF is a Bug Bounty?](https://www.ceos3c.com/hacking/ethical-hacking-diaries-1-wtf-is-a-bug-bounty/) - by ceos3c
- [How to Set up Certificate-Based SSH for Bug Hunting](https://medium.com/@c0ldbr3w/how-to-set-up-certificate-based-ssh-for-bug-hunting-bonus-ef4af95fca05) - by Mack Staples
- [XSS in Google Colaboratory + CSP bypass](https://blog.bentkowski.info/2018/06/xss-in-google-colaboratory-csp-bypass.html) by Michał Bentkowski
- [Zseano’s notes on hacking & mentoring](https://blog.intigriti.com/2020/04/29/bug-business-3-zseanos-notes-on-hacking-mentoring/) by Intigriti & Zseano
- [MY BUG BOUNTY JOURNEY!](https://www.youtube.com/watch?v=ug7FzoByLFc) by Farah Hawa
## XSS
You can find a ton of awesome XSS reports by searching through the HackerOne Hacktivity Page (https://hackerone.com/hacktivity?querystring=XSS). Here are some more complex and some of my favorite XSS related blog posts:

- [XSS on Google Search - Sanitizing HTML in The Client?](https://www.youtube.com/watch?v=lG7U3fuNw3A) - LiveOverflow
    - [The Fix](https://github.com/google/closure-library/commit/c79ab48e8e962fee57e68739c00e16b9934c0ffa)
- [Cracking my windshield and earning $10,000 on the Tesla Bug Bounty Program](https://samcurry.net/cracking-my-windshield-and-earning-10000-on-the-tesla-bug-bounty-program/) - [Sam Curry](https://twitter.com/samwcyo)
- [Effortlessly finding Cross Site Script Inclusion (XSSI) & JSONP for bug bounty](https://medium.com/bugbountywriteup/effortlessly-finding-cross-site-script-inclusion-xssi-jsonp-for-bug-bounty-38ae0b9e5c8a) - [@th3_hidd3n_mist](https://twitter.com/th3_hidd3n_mist)
- [Microsoft Edge (Chromium) - EoP via XSS to Potential RCE](https://leucosite.com/Edge-Chromium-EoP-RCE/) - [@Qab](https://twitter.com/qab)
- [Reflected XSS in https://blocked.myndr.net](https://hackerone.com/reports/824433) - Thilakesh
- [Google Bug Bounty Writeup- XSS Vulnerability](https://pethuraj.com/blog/google-bug-bounty-writeup/) - [@itsmepethu](https://twitter.com/itsmepethu)
- [How to solve the INTIGRITI Easter XSS challenge using only Chrome Devtools](https://www.youtube.com/watch?v=IhPsBMBDFcg) - by STÖK
- [Found Stored Cross-Site Scripting — What’s Next? — Privilege Escalation like a Boss](https://medium.com/bugbountywriteup/found-stored-cross-site-scripting-whats-next-privilege-escalation-like-a-boss-d-8fb9e606ce60) - by Harsh Bothra
- [Bypassing WAF to perform XSS](https://medium.com/bugbountywriteup/bypassing-waf-to-perform-xss-2d2f5a4367f3) - by Kleitonx00


### DOM XSS
- [Persistent DOM-based XSS in https://help.twitter.com via localStorage](https://hackerone.com/reports/297968) - harisec
- [DOM based XSS in search functionality](https://hackerone.com/reports/168165) - sameoldstory
- [A Tale Of A DOM Based XSS In Paypal](https://www.rafaybaloch.com/2017/06/a-tale-of-dom-based-xss-in-paypal.html) - Rafay Baloch
- [H1514 DOMXSS on Embedded SDK via Shopify.API.setWindowLocation abusing cookie Stuffing](https://hackerone.com/reports/422043) - filedescriptor
- [DOM XSS on app.starbucks.com via ReturnUrl](https://hackerone.com/reports/526265) - Gamer7112
### Stored XSS
- [Another XSS in Google Colaboratory](https://blog.bentkowski.info/2018/09/another-xss-in-google-colaboratory.html) - Michał Bentkowski
- [Google adwords 3133.7$ Stored XSS](https://medium.com/@Alra3ees/google-adwords-3133-7-stored-xss-27bb083b8d27) - Emad Shanab
- [Stored XSS on Facebook](https://opnsec.com/2018/03/stored-xss-on-facebook/) - Enguerran Gillier
- [Yahoo Mail stored XSS](https://klikki.fi/adv/yahoo.html) - Jouko Pynnönen
- [Yahoo Mail stored XSS #2](https://klikki.fi/adv/yahoo2.html) - Jouko Pynnönen
- [Account Recovery XSS](https://sites.google.com/site/bughunteruniversity/best-reports/account-recovery-xss) - Gábor Molnár

## SSRF
- [DEF CON 27 Conference - Ben Sadeghipour - Owning The Clout Through Server Side Request Forgery](https://www.youtube.com/watch?v=o-tL9ULF0KI)<br>- Nahamsec & daeken | DEFCON 2019
- [Piercing The Veil: Server Side Request Forgery Attacks On Internal Networks](https://peertube.opencloud.lu/videos/watch/40f39bfe-6d3c-40f5-bcab-43f20944ca6a)<br>- Alyssa Herrera | Hack.lu 2019
- [Vimeo upload function SSRF](https://medium.com/@dPhoeniixx/vimeo-upload-function-ssrf-7466d8630437) - Sayed Abdelhafiz
- [Piercing the Veal](https://medium.com/@d0nut/piercing-the-veal-short-stories-to-read-with-friends-4aa86d606fc5) - by d0nut
- [MY EXPENSE REPORT RESULTED IN A SERVER-SIDE REQUEST FORGERY (SSRF) ON LYFT](https://www.nahamsec.com/posts/my-expense-report-resulted-in-a-server-side-request-forgery-ssrf-on-lyft) - by nahamsec


## Vulnerability Scanning
- [NMAP For Vulnerability Discovery](https://www.peerlyst.com/posts/nmap-for-vulnerability-discovery-sachin-wagh) - Sachin Wagh

## Token / Authentication
- [Abusing feature to steal your tokens](https://medium.com/@rootxharsh_90844/abusing-feature-to-steal-your-tokens-f15f78cebf74) - Harsh Jaiswal
- [How I was able to bypass OTP code requirement in Razer [The story of a critical bug]](https://medium.com/bugbountywriteup/how-i-was-able-to-bypass-otp-token-requirement-in-razer-the-story-of-a-critical-bug-fc63a94ad572?) - Ananda Dhakal
- [Bypassing GitHub's OAuth flow](https://blog.teddykatz.com/2019/11/05/github-oauth-bypass.html) - [@not_aardvark](https://twitter.com/not_aardvark)
- [Subdomain Takeover to Authentication bypass](https://hackerone.com/reports/335330) - by geekboy


## SQL Injection
- [Time-Based Blind SQL Injection In GraphQL](https://medium.com/bugbountywriteup/time-based-blind-sql-injection-in-graphql-39a25a1dfb3c) - Divyanshu Shukla
- [SQL Injection Extracts Starbucks Enterprise Accounting, Financial, Payroll Database](https://hackerone.com/reports/531051) - spaceraccoon
- [Finding SQL injections fast with white-box analysis — a recent bug example](https://medium.com/@frycos/finding-sql-injections-fast-with-white-box-analysis-a-recent-bug-example-ca449bce6c76?) - [@frycos](https://twitter.com/frycos)
- [How we hacked one of the worlds largest Cryptocurrency Website](https://strynx.org/insecure-crypto-code-execution/) - [strynx](https://strynx.org/)
- [Blind SQL Injection on windows10.hi-tech.mail.ru](https://hackerone.com/reports/786044) - Просто душка (api_0)
- [How to Hack Database Links in SQL Server!](https://blog.netspi.com/how-to-hack-database-links-in-sql-server/) - Antti Rantasaari

## Mobile
### iOS
- [From checkra1n to Frida: iOS App Pentesting Quickstart on iOS 13](https://spaceraccoon.dev/from-checkra1n-to-frida-ios-app-pentesting-quickstart-on-ios-13) - spaceraccoon
### Android
- [A deep dive into reversing Android pre-Installed apps](https://github.com/maddiestone/ConPresentations/blob/master/Blackhat2019.SecuringTheSystem.pdf) and the [BlackHat Talk](https://www.youtube.com/watch?v=U6qTcpCfuFc) - Maddie Stone

## HTTP Desync
- [HTTP Desync Attacks: Request Smuggling Reborn](https://portswigger.net/research/http-desync-attacks-request-smuggling-reborn) in combination with this [report](https://hackerone.com/reports/510152) - [James Kettle](https://twitter.com/albinowax)
- [HTTP Request Smuggling on vpn.lob.com](https://hackerone.com/reports/694604) - 0X0 (painreigns)
- [Mass account takeovers using HTTP Request Smuggling on https://slackb.com/ to steal session cookies](https://hackerone.com/reports/737140) - Evan Custodio

## File Upload
- [Webshell via File Upload on ecjobs.starbucks.com.cn](https://hackerone.com/reports/506646) - johnstone
- [Facebook Messenger server random memory exposure through corrupted GIF image ](https://www.vulnano.com/2019/03/facebook-messenger-server-random-memory.html) - [@xdzmitry](https://twitter.com/xdzmitry)
- [A Tale of Exploitation in Spreadsheet File Conversions](https://buer.haus/2019/10/18/a-tale-of-exploitation-in-spreadsheet-file-conversions/) - [@bbuerhaus](https://twitter.com/bbuerhaus)//[@daeken](https://twitter.com/daeken)//[@erbbysam](https://twitter.com/erbbysam)//[@smiegles](https://twitter.com/smiegles)
- [External XML Entity via File Upload (SVG)](https://0xatul.github.io/posts/2020/02/external-xml-entity-via-file-upload-svg/) - by 0xatul


## Automation
- [Fasten your Recon process using Shell Scripting](https://medium.com/bugbountywriteup/fasten-your-recon-process-using-shell-scripting-359800905d2a) - Mohd Shibli
- [Beginner’s Guide to recon automation](https://medium.com/bugbountywriteup/beginners-guide-to-recon-automation-f95b317c6dbb) - Ashish Jha
- [Burp Suite tutorial: IDOR vulnerability automation using Autorize and AutoRepeater (bug bounty)](https://www.youtube.com/watch?v=3K1-a7dnA60) - STÖK & Fisher
- [gitGraber: A tool to monitor GitHub in real-time to find sensitive data](https://blog.yeswehack.com/2019/10/08/gitgraber-a-tool-to-monitor-github-in-real-time-to-find-sensitive-data/) - by [@adrien_jeanneau](https://twitter.com/adrien_jeanneau) & [@R_Marot](https://twitter.com/R_marot)

## Buffer Overflow
- [Filling in the Blanks: Exploiting Null Byte Buffer Overflow for a $40,000 Bounty](https://samcurry.net/filling-in-the-blanks-exploiting-null-byte-buffer-overflow-for-a-40000-bounty/) - [Sam Curry](https://twitter.com/samwcyo)
- [Writing a Simple Buffer Overflow Exploit](https://www.youtube.com/watch?v=oS2O75H57qU) - LiveOverflow

## IDOR
- [Steal Earning of Airbnb hosts by Adding Bank Account/Payment Method](https://www.indoappsec.in/2019/12/airbnb-steal-earning-of-airbnb-hosts-by.html) - [Vijay Kumar ](https://twitter.com/IndoAppSec)
- [GraphQL IDOR leads to information disclosure](https://medium.com/@R0X4R/graphql-idor-leads-to-information-disclosure-175eb560170d) - [@R0X4R](https://twitter.com/R0X4R)
- [From Multiple IDORs leading to Code Execution on a different Host Container](https://www.rahulr.in/2019/10/idor-to-rce.html?m=1) - [@Rahul_R95](https://twitter.com/Rahul_R95)
- [Automating BURP to find IDORs](https://medium.com/cyberverse/automating-burp-to-find-idors-2b3dbe9fa0b8) - [Aditya Soni](https://medium.com/@hetroublemakr)

## GraphQL
- [Private System Note Disclosure using GraphQL](https://hackerone.com/reports/633001) - Ron Chan
- [Graphql Abuse to Steal Anyone’s Address](https://blog.usejournal.com/graphql-bug-to-steal-anyones-address-fc34f0374417) - pratik yadav
 - [Email address of any user can be queried on Report Invitation GraphQL type when username is known](https://hackerone.com/reports/792927) - msdian7

## RCE
- [My First RCE (Stressed Employee gets me 2x bounty)](https://medium.com/@abhishake100/my-first-rce-stressed-employee-gets-me-2x-bounty-c4879c277e37) - [Abhishek Yadav](https://medium.com/@abhishake100)
- [How dangerous is Request Splitting, a vulnerability in Golang or how we found the RCE in Portainer and hacked Uber](https://medium.com/@andrewaeva_55205/how-dangerous-is-request-splitting-a-vulnerability-in-golang-or-how-we-found-the-rce-in-portainer-7339ba24c871) - by Andrewaeva

## Recon
- [Subdomain Recon Using Certificate Search Technique](https://www.r00tpgp.com/2020/01/subdomain-recon-using-certificate.html?m=0)
- [Notes about Nahamsecs Recon Sessions](https://mavericknerd.github.io/knowledgebase/nahamsec/recon_session_1/) - [maverickNerd](https://github.com/maverickNerd)
- [10 Recon Tools For Bug Bounty](https://medium.com/@hackbotone/10-recon-tools-for-bug-bounty-bafa8a5961bd) - Anshuman Pattnaik
- [Recon: Create a methodology and start your subdomain enumeration](https://failednuke.info/2020/recon-create-a-methodology-and-start-your-subdomain-enumeration/) - by FailedNuke
- [THEY SEE ME SCANNIN’, THEY HATIN’: A BEGINNER’S GUIDE TO NMAP](https://securityqueens.co.uk/they-see-me-scannin-they-hatin-a-beginners-guide-to-nmap/) - by Sophia (https://twitter.com/SecQueens)

## Smart Contracts
- [Steal collateral during `end` process, by earning DSR interest after `flow](https://hackerone.com/reports/672664)(Listed as Business Logic Error)
- [Steal all MKR from `flap` during liquidation by exploiting lack of validation in `flap.kick`](https://hackerone.com/reports/684152)(Listed as Improper Input Validation)

## API
- [31 Days of API Security Tips](https://github.com/smodnix/31-days-of-API-Security-Tips) - [smodnix](https://github.com/smodnix)

## Misc
- [Hacking GitHub with Unicode's dotless 'i'](https://eng.getwisdom.io/hacking-github-with-unicode-dotless-i/)
- [Abusing autoresponders and email bounces](https://medium.com/intigriti/abusing-autoresponders-and-email-bounces-9b1995eb53c2) - securinti
- [Abusing HTTP hop-by-hop request headers](https://nathandavison.com/blog/abusing-http-hop-by-hop-request-headers) - [@nj_dav](https://twitter.com/nj_dav)
- [Cracking reCAPTCHA, Turbo Intruder style](https://portswigger.net/research/cracking-recaptcha-turbo-intruder-style) - James Kettle
- [Abusing ImageMagick to obtain RCE](https://strynx.org/imagemagick-rce/) - [strynx](https://strynx.org/)
- [How to Get a Finger on the Pulse of Corporate Networks via the SSL VPN](https://blog.detectify.com/2019/09/19/alyssa-herrera-pulse-corporate-networks-ssl-vpn/) - [Alyssa Herrera](https://twitter.com/Alyssa_Herrera_)
- [2 Cases of Path Traversal](https://jlajara.gitlab.io/posts/2020/03/29/Path_Traversal.html) by [@leonishan_](https://twitter.com/leonishan_)
- [Top 10 web hacking techniques of 2019](https://portswigger.net/research/top-10-web-hacking-techniques-of-2019) by [James Kettle](https://twitter.com/albinowax)
- [Understanding Search Syntax on Github](https://help.github.com/en/github/searching-for-information-on-github/understanding-the-search-syntax#exclude-certain-results) by Github
- [URL link spoofing (Slack)](https://hackerone.com/reports/481472) by Akaki Tsunoda (akaki)
- [Abusing HTTP Path Normalization and Cache Poisoning to steal Rocket League accounts](https://samcurry.net/abusing-http-path-normalization-and-cache-poisoning-to-steal-rocket-league-accounts/) by Sam Curry
- [The Secret sauce of bug bounty](https://medium.com/bugbountywriteup/the-secret-sauce-of-bug-bounty-bdcc2e2d45af) by Mohamed Slamat


---
back to [Intro Page](/README.md)