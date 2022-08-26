# Web-Application-Security

![app-security](https://user-images.githubusercontent.com/84139300/186833699-81e93f22-47bd-4e39-b86a-cf1b2922c949.jpg)


   WEB APPLICATION :A web application (or web app) is application software that runs in a web browser, unlike software programs that run locally  on the operating system (OS) of the devices. Web applications are delivered on the World Wide Web (WWW)  to users with an active network connection.

WEB APPLICATION SECURITY :Web application security is a central component of any web-based business.  Web application security deals specifically with the security surrounding websites, web applications and web services such as APIs.

What are common web app security vulnerabilities?

= Attacks against web apps range from targeted database manipulation to large-scale network distruction 

Web application hacking involves the attacker exploiting vulnerabilities with in the web application. These vulnerabilities are documented as OWASP Top 10 vulnerabilities such as :

check this link👇

↪ https://askmitra.com/owasp-what-are-the-owasp-top-10-vulnerabilities-for-2021-whitehat-top-40-vulnerabilitiesexplaination/

↪ A web application security experts job is to ensure the security of the application by performing penetration testing on various levels before deploying the application or while maintaining it.

↪ I think web application is depend on website and app ta app vaihalyo. Logically vannu parda web application website based vayepaxi websitema hamile post gareko kehi things tyo app ma pani automatically posted huneynai vayo (hunxa hola hai malai ali tha xaina). In case website appma hosted xa vaney hunxa. Web hacking & Web application hacking ma teti difference xaina aba application ma painey pani tei bug ho websitema painey pani tei bugs/vulnerabilities ho.

↪ How to do it ??

- pahila suru web-application / website lai ramro sanga analysis garnu paryo.

- tyo websitema kun server use garyaxa check garnu paryo.

- database server kun xa & kun query language use garyaxa sql & mysql ??

- sitemap check garnu paryo. yo vaneko websiteko purai map matlab tesma k k xa contents kasto xa tyo check garne.

- kun programming language used vaxa ??

- Reconnaissance garnu paryo.

↪ https://askmitra.com/reconnaissance-vaneko-k-ho-and-yeslai-kasari-garna-sakinxata/

- espaxi tapailai tha huna sakxa webserver / website ma euta matra website hudaina tesma thuprai subdomains pani hunxa  hamile teslai exolore garnu paryo.

- Alot of big website when they are try to install and add the new features in the website they install in a subdomain such as eg. beta.facebook.com, it actually contains beta version of facebook which contain experimental features of facebook and there are highly chance to finding vulnerability in them and this is actually true now so long someone is able bruteforce the restore password key for any facebook users and this was only possible users through the beta of facebook.com. The beta usually contains more problems in normal website so there will be useful to try and hack into it.

- For finding subdomains of a target website you can use knock tool and run it.

- For finding hidden files+directories of a targeted webserver you can use dirb tool.

- dirb install garera 👉 command usage = dirb [target] [wordlist] [options]
- optionsko lagi help command use garne

- eg. dirb https://m.facebook.com

- After discovering sensitive files using dirb tool, we will explore the terminal results, by comping  by one and pasting in google or any search engines.

- In terminal somewhere if you found  /phpinfo.php in url in terminal, this files is very useful because it displays all information about php interptre running in the webserver.

- You can also find admim pannel to login into database.

- Another one you can also found /robots.txt file : This is the files that tells search engine how to deal with website, usually it contains password files that we don't want to see website on google to read.

- And then the website is also vulnerable with file upload vulnerabilities.
👉 It is simple types of vulnerabilities, If any website is vulnerable with this vulnerability in case it allows upload any type of files. Eg. the target website understand php then we can upload any php file and php shell and get full control over the target website. For creating shell we can use python code, ruby shell and php shell.

- You can also make php shell or backdoor using weevly tool.
👉 command ussage : weevely generate 123456 /root /shell.php

👉Note : 123456 : password

- After that the backdoor / shell will be generated.

- Then upload the php shell in victim site and after uploaded type/shell.php in url bar and copy the whole url and type in terminal weevely and paste the url and set password and hit enter. After that, you can type linux any commands in terminal and then the commands will executed in target webserver.

