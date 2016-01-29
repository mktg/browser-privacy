Links to web browser privacy and hardening resources, as well as browser fingerprinting and identification developer tools. Private and state organizations monitor and record your online activities, so do google, bing, yanded, yahoo, baidu, facebook, and a million others. These are useful resources I've come across while making lots of, err, accounts.
  
This list will mostly focus on browsers, browser configs and browser fingerprinting. [Tor](https://www.torproject.org/projects/torbrowser.html.en) [resources](https://www.torproject.org/projects/projects.html.en) [intentionally](http://the-hidden-wiki.com/) [omitted](http://the-hidden-wiki.com/).

## Alternative Browsers ##

- [SRWare Iron (Chrome)](http://www.srware.net/en/software_srware_iron.php) Chrome with the eye of sauron removed.
- [Pale Moon (Firefox)](https://www.palemoon.org/) Custom-built and optimized Mozilla Firefox browsers for Windows Operating Systems.
- [Midori](http://www.midori-browser.org/) Yay more open source webkit.
----------

## Chrome extensions ##
- [CanvasFingerprintBlock](https://chrome.google.com/webstore/detail/canvasfingerprintblock/ipmjngkmngdcdpmgmiebdmfbkcecdndc) - Does what it says on the tin.
- [Scriptsafe](https://chrome.google.com/webstore/detail/scriptsafe/oiigbmnaadbkfbmpbfijlflahbdbdgdf) - For various values of safe.
- [Ublock](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm/related) Less terrible than adblock plus. WebRTC blocking doesn't work because 
- [uMatrix](https://chrome.google.com/webstore/detail/umatrix/ogfcmafjalglgifnmanfmnieipoejdcf) Content blocking overkill

## Chrome Config ##
	chrome://flags/#disable-webrtc  (doesn't work, do your spamming in another browser)


----------

## Firefox Config / Profile software ##
Firefox is a bit of a dog, but it's certainly less invasive than modern chrome builds.
- [ConfigFox](http://configfox.sourceforge.net/) - A utility to manage Firefox advanced, hidden settings and tweaks, mostly concerning security and privacy.
- [Firefox Profilemaker](https://www.ffprofile.com/) [Github](https://github.com/allo-/firefox-profilemaker) - Makes FF profiles with secure/private defaults. 
- [Firefox Environment Backup Extension](http://softwarebychuck.com/febe/febe.html#latest)  - FEBE allows you to quickly and easily backup your Firefox extensions. Rebuilds your extensions individually into installable .xpi files. 


## Firefox Config / Tweaks ##
- [Firefox bullshit removal via about:config](https://gist.github.com/haasn/69e19fc2fe0e25f3cff5) - Lots of config tweaks with explanations
- [Firefox Hardening](https://github.com/pyllyukko/user.js/) - This user.js is a bit over the top to be useable day to day, but it's a good start.

## Firefox about:config tweaks ##
    	media.peerconnection.enabled;false // disable webrtc
    	media.peerconnection.turn.disable;true // disable webrtc
    	media.peerconnection.use_document_iceservers;false // disable webrtc
    	media.peerconnection.video.enabled;false // disable webrtc
    	media.peerconnection.identity.timeout;1 // disable webrtc

----------


## Browser Abuse ##
- [BeEF - The Browser Exploitation Framework Project](http://beefproject.com/)    / https://github.com/beefproject/beef.
- [Sniffing browser history using HSTS + CSP](https://github.com/diracdeltas/sniffly) -  [Demo](http://zyan.scripts.mit.edu/sniffly/).

## Browser Leak Tests ##
- [http://browserspy.dk/](http://browserspy.dk/)
- [https://www.browserleaks.com/](https://www.browserleaks.com/)
- [https://panopticlick.eff.org/](https://panopticlick.eff.org/)
- [https://ipleak.net/](https://ipleak.net/)
- [http://www.dnsleaktest.com/](http://www.dnsleaktest.com/) DNS Leaks test .
- [https://www.grc.com/dns/dns.htm](https://www.grc.com/dns/dns.htm) Another DNS Leaks test .


----------


## Web tracking, Browser fingerprinting & Analytics libraries ##
-[Evercookie](https://github.com/samyk/evercookie) - Produces extremely persistent, respawning cookies in a browser.
- [Google Analytics](https://analytics.google.com/) It's kinda scary how much data they collect daily.
- [fingerprintjs2](https://github.com/Valve/fingerprintjs2) - Modern & flexible browser fingerprinting library, a successor to the original fingerprintjs.
- [UserAgentInfo](https://github.com/quentin389/UserAgentInfo) - PHP class for parsing user agent strings (HTTP_USER_AGENT). Includes mobile checks, bots and banned bots checks, browser types/versions and more.
- [http://mobiledetect.net/](http://mobiledetect.net/) Mobile Detect is a lightweight PHP class for detecting mobile devices (including tablets). Stacks of plugins.
- [Browscap](http://tempdownloads.browserscap.com/) - browscap contains a huge database of incredibly detailed specific user agents information but it sucks with newer user agents and sucks even more for mobile detection.

## DNS Servers ##
-  **OpenDNS**
 - 208.67.222.222 , 208.67.220.220
-  **Level 3**
	-  209.244.0.3 , 209.244.0.4 , 4.2.2.1 , 4.2.2.2 , 4.2.2.3 , 4.2.2.4
-	**[Comodo Secure DNS](https://www.comodo.com/secure-dns/)**
	-	8.26.56.26 , 8.20.247.20
-	**[DNS Watch](https://dns.watch/index)**
	-	82.200.69.80 , 84.200.70.40
		resolver1.dns.watch , resolver2.dns.watch
	- `2001:1608:10:25::1c04:b12f ` ,   `2001:1608:10:25::9249:d69b`
	resolver1.dns.watch , resolver2.dns.watch 


-  **Google** *Argurably better than your local dictatorship's honeypot, but still f*cking google.*
	-  8.8.8.8 , 8.8.4.4



## Proxy Providers ##
- [SSL Private Proxy](https://www.sslprivateproxy.com) All sorts of great stuff.
- [Squid Proxies](http://www.squidproxies.com/) Very fast proxies.
- [Fineproxy.org](https://buy.fineproxy.org/eng/mini.html) Good for cheap and short term proxies.

## Further Links ##
- [privacytools.io](https://www.privacytools.io/) Privacytools.io provides knowledge and tools to protect your privacy .against global mass surveillance. Because as it turns out, they really are watching.
- [OS-X-Security-and-Privacy-Guide](https://github.com/drduh/OS-X-Security-and-Privacy-Guide)  - This is a collection of thoughts on securing a modern Apple Mac computer using OS X 10.11 "El Capitan", as well as steps to improving online privacy.

## Papers ##
- [Client Fingerprinting via Analysis of Browser Scripting Environment](https://www.sans.org/reading-room/whitepapers/testing/client-fingerprinting-analysis-browser-scripting-environment-33503) 
	- https://www.sans.org/reading-room/whitepapers/testing/client-fingerprinting-analysis-browser-scripting-environment-33503 . 
- **[The Web Never Forgets: Persistent Tracking Mechanisms in the Wild](https://securehomes.esat.kuleuven.be/~gacar/persistent/) **
	- https://securehomes.esat.kuleuven.be/~gacar/persistent/the_web_never_forgets.pdf
- [New browser fingerprinting tricks](https://zyan.scripts.mit.edu/presentations/toorcon2015.pdf) / http://zyan.scripts.mit.edu/sniffly
