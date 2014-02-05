killer-htaccess
===============

Secure your server, protect your web apps, load your sites faster, avoid malware, block malicious code, be Happy

Content
-------


Apache htaccess rules to protect from DoS, Sql Injection, XSS and block bad bots.

PROTECT
-------

Kill them all!:

- E-mail harvesters
- Content scrapers
- Spam bots
- Vulnerability scanners
- Aggressive bots that provide little value
- Bots linked to viruses or malware
- Government surveillance bots
- Russian search engine Yandex
- Chinese search engine Baidu




SQL Injection Protection Attacks on web applications
----------------------------------------------------

SQL Injection is a code injection technique, used to attack data driven applications, in which malicious SQL statements are inserted into an entry field for execution (e.g. to dump the database contents to the attacker)
[SQL Injection Attack](http://en.wikipedia.org/wiki/SQL_injection),




Protection XSS Attacks on web applications
------------------------------------------

XSS enables attackers to inject client-side script into Web pages viewed by other users. A cross-site scripting vulnerability may be used by attackers to bypass access controls such as the same origin policy
[XSS Attack](http://en.wikipedia.org/wiki/Cross-site_scripting),




Yandex/Baidu
------------

Unless your website is written in Russian or Chinese, you probably don't
get any traffic from them. They mostly just waste bandwidth and consume resources.


Bots Are Liars
--------------

Bots try to make themselves look like other software by disguising their
useragent. Their useragents may look harmless, perfectly legitimate even.
For example, "^Java" but according to
[Project Honeypot](https://www.projecthoneypot.org/harvester_useragents.php),
it's actually one of the most dangerous.


Setup
-----

If you have a bizarre or complicated setup, be sure to look everything
over before using it. But for anyone with something that resembles
a standard Apache installation, this should work without any issues.

Xtras
-----

Run this cmd in your shell to find malicious scripts in your server

[$>grep -RPnDskip "(passthru|shell_exec|system|phpinfo|base64_decode|chmod|mkdir|fopen|fclose|readfile) *\(" /var/www/vhosts/myhost.com.co/httpdocs/ >sospechosos.txt]

