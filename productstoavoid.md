# 24 Hour Support Wiki

[Return to main wiki page](https://github.com/CommandMC/24HS-Wiki/blob/main/index.md)
 
## Products to avoid

**Disclaimer:** These are personal opinions of the staff  
While these are our personal opinions, discussions are more than welcome. Feel free to join [our Discord server](https://discord.gg/VS5wq89) and ping the `Feel free to Ping` role with your ideas and suggestions.

Contributors: All sources used here **must** be archived by the [Wayback machine](https://web.archive.org/) to prevent broken links. Linking to the original source is fine as long as you made sure the source is archived.

---
### Any Driver Updater software 

This includes Snappydriver, iOBIT driver booster, CCleaner, DriversCloud, DriverMax, Driver Easy, VueScan, Driver Genius, Driver Reviver, Driver Support, Smart Driver Updater, ...  
**Any and all driver updater software should not be used.**

* Windows Updates provides all security and driver updates needed most of the time, those not provided are available through your manufacturer's website, which are tested to work.
* Driver Updater software is almost always closed source, you have no way to verify if it is legitimately only doing what you ask it to do.

#### Recommended alternatives

* Wait for Windows updates to provide updates for you, these will be tested to work with your configuration
* Go to your manufacturer's website for drivers. Generally only drivers you ever have to manually update are your GPU drivers. If you have an Nvidia card you can install [Geforce Experience](https://www.nvidia.com/en-us/geforce/geforce-experience/download/)
  if you do not have it downloaded already, then go to settings and enable desktop notifications to notify you when an update is available.
  For CPU chipset drivers, see [this Wiki](https://github.com/CommandMC/24HS-Wiki/blob/main/systemuptodate.md#chipset-drivers)

---
### Any System "Optimizer", "System care" or "Fixer"

* Windows takes care of itself. Do you really believe anyone other than the makers know Windows better?
* These so-called "system optimizers" [use intentional false positives to convince users that their systems have problems. Then they try to sell you their software, claiming it will remove these problems.](https://blog.malwarebytes.com/cybercrime/2015/06/digital-snake-oil/)
* [DLL Fixer injects you with malware](https://forums.malwarebytes.com/topic/262528-removal-instructions-for-dll-files-fixer/)
* Everything from iOBIT is not advised.  
  IObit Malware Fighter [scores terribly in malware protection tests, has no results from independent labs, and does more harm than good](https://www.pcmag.com/reviews/iobit-malware-fighter-pro).
  Advanced System Care is classified as a [PUP by Malwarebytes](https://forums.malwarebytes.com/topic/198901-advanced-system-care-pup/?tab=comments#comment-1115452).
  iObit Uninstaller is closed source which has [better alternatives](https://www.bcuninstaller.com/), it also includes [BrowseFox adware](https://www.virustotal.com/en/file/e14099db4fc0a7c0ca2eefec7c5864a8799d4f93cbb0f08709345e93df222640/analysis/1451580689/).
  iOBit has also [stolen Malwarebytes intellectual properly, including it in their own product as their own](https://forums.malwarebytes.com/topic/29681-iobit-steals-malwarebytes-intellectual-property/)

#### Recommended alternatives

* Windows takes care of itself, if your computer is acting slowly try seeing [what you have setup to launch at startup](https://support.microsoft.com/en-us/windows/change-which-apps-run-automatically-at-startup-in-windows-10-9115d841-735e-488d-e749-9ba301d441e6/).
  For more support feel free to join [our Discord server](https://discord.gg/VS5wq89).

---
### CCleaner

* CCleaner has been caught [harvesting data from users](https://www.ghacks.net/2018/08/01/ccleaner-5-45-dont-install),
  has been [compromised to distribute Malware](https://www.bleepingcomputer.com/news/security/ccleaner-compromised-to-distribute-malware-for-almost-a-month/),
  then began [installing their parent's company's AV without a user's input](https://www.techspot.com/news/77949-ccleaner-could-install-avast-anti-virus-without-permission.html)
* Registry Cleaners, or any sort of cache cleaner is completely unnecessary. Windows takes care of itself. Do you really believe anyone other than the makers know Windows better?
  Microsoft themselves [state registry cleaners, such as CCleaner, only do harm](https://support.microsoft.com/en-us/help/2563254/microsoft-support-policy-for-the-use-of-registry-cleaning-utilities)
* [CCleaner has been caught installing Avast without permission](https://www.techspot.com/news/77949-ccleaner-could-install-avast-anti-virus-without-permission.html)

#### Recommended alternatives

* Only "useful" feature of CCleaner would be the ability to clear cache of applications. While this can be done manually in all of them, if you want an automated tool use [BleachBit](https://www.bleachbit.org/)
  which is [completely open source](https://github.com/bleachbit/bleachbit).
* Alternative would be to simply clear cache manually: [Firefox](https://support.mozilla.org/en-US/kb/how-clear-firefox-cache), [Google Chrome](https://support.google.com/accounts/answer/32050?co=GENIE.Platform%3DDesktop&hl=en),
  and most software has instructions on how to do so.

---
### µTorrent, BitComet, BitLord, BitTorrent

* These four are NOT open source. There is no way to verify what they are doing and how they are doing it.
* µTorrent has been caught deliberately [installing toolbars in your browser](https://torrentfreak.com/utorrent-browser-toolbar-mystery-causes-havoc-among-users-101218),
  includes [adware](https://www.pcmag.com/archive/utorrent-updates-software-to-include-ads-301477),
  has [been caught installing cryptocurrency miners](https://www.theverge.com/2015/3/6/8161251/utorrents-secret-bitcoin-miner-adware-malware),
  and [switched Russian and Ukranian users to the Yandex browser without user input](https://xakep.ru/2013/10/26/61491)
* BitComet is currently [collecting data on what users download using their client](https://en.wikipedia.org/wiki/BitComet#Hash_reporting).
* BitLord [has reports of installing adware/malware](https://old.reddit.com/r/torrents/comments/6ynhy9/is_bitlord_safe_to_download_things/dmopupk)
* BitTorrent (client) is made by the same people of µTorrent.

#### Recommended alternatives

Note: We are not responsible for any laws or regulations you break. **You** are responsible for verifying if using BitTorrent clients is legal. We are not lawyers.  
Using any of these clients is not a substitute for using a [good VPN](https://github.com/CommandMC/24HS-Wiki/blob/main/productstoavoid.md#any-and-all-free-vpns).

Good alternatives include the following, all of which are open source, basically means you can look at the source code for a program. This means you can modify it to suit your purposes. 
It also means you can verify what it does, make sure there isn't any unsecure/malicious code or backdoors, etc.

* [qBittorrent](https://github.com/qbittorrent/qBittorrent/releases), it is currently developed by contributors worldwide and is funded ONLY through donations. [Be sure to bind qBittorrent to the VPN client you are using to prevent leaks](https://www.ghacks.net/2016/03/23/qbittorrent-block-transfers-vpn-disconnect/)
* [Transmission](https://transmissionbt.com), it is the default BitTorrent client of many distributions (including popular ones such as Ubuntu, Mint and Fedora). 
* [BiglyBT](https://www.biglybt.com), the newest client, released only in 2017. 

Not much differentiates these three, all are solid choices. Recommended to try qBittorrent first, as that has the most community backing. 

---
### Any and ALL Free VPNs

* There is no such thing as a free VPN. You are paying for it somehow. Servers are not free to maintain. If you are not the customer, you are the product.
  There is no proof of free VPNs protecting their "customers" data, yet there is countless [investigations proving they sell their "customers" data to advertisers, and anyone who pays enough](https://www.top10vpn.com/free-vpn-app-investigation).
  There has been [countless instances](https://www.comparitech.com/blog/vpn-privacy/ufo-vpn-data-exposure) of supposedly [no log VPNs](https://vpnpro.com/blog/hidden-vpn-owners-unveiled-97-vpns-23-companies)
  not providing what they promised. Seriously, [there's a lot](https://vpnpro.com/blog/chinese-company-secretly-behind-popular-apps-seeking-dangerous-permissions).
* No free VPN undergoes a audit that independently verifies their claim of no logs is accurate, most legitimate VPNs [do indeed](https://cure53.de/pentest-report_mullvad_v2.pdf) go through independent audits.
  This is important as [studies have shown audits would've caught issues that affected customers](https://www.zdnet.com/article/nordvpn-http-post-bug-exposed-sensitive-customer-information)
* Most free VPNs don't publicly shares who they are. You wouldn't trust your finances to someone with a fake identity, so why trust them with your internet life? 
* This is not the early 2000s, there are plenty of VPNs that are [cheap and good](https://mullvad.net)

#### Recommended alternatives

Note: We are not responsible for any laws or regulations you break. **You** are responsible for verifying if using a VPN, Tor, or any circumvention of censorship is legal. We are not lawyers.  

* [Mullvad](https://mullvad.net)'s VPN clients have been audited by Cure53 and Assured AB in a pentest report published at cure53.de. The security researchers concluded:
  [Cure53 and Assured AB are happy with the results of the audit and the software leaves an overall positive impression. With security dedication of the in-house team at the Mullvad VPN compound, the testers have no doubts about the project being on the right track from a security standpoint.](https://cure53.de/pentest-report_mullvad_v2.pdf).
  They provide the [full source code for all their clients](https://github.com/mullvad). They are also very reasonable on their monthly costs, and accept MULTIPLE forms of payment, including cash mailed in an envelope! Mullvad also comes with a kill switch that you can turn on or off at will.
* [IVPN](https://www.ivpn.net) [has undergone a no-logging audit from Cure53 which concluded in agreement with IVPN's no-logging claim. IVPN has also completed a comprehensive pentest report Cure53 in January 2020. IVPN has also said they plan to have annual reports in the future.](https://cure53.de/summary-report_ivpn_2019.pdf).
  As of Feburary 2020 IVPN applications are now [open source. Source code can be obtained from their GitHub organization.](https://www.ivpn.net/blog/ivpn-applications-are-now-open-source).

Provided you're using qBittorrent, be sure to [bind it to the VPN client you are using to prevent leaks](https://www.ghacks.net/2016/03/23/qbittorrent-block-transfers-vpn-disconnect/)

* [Tor Browser](https://www.torproject.org/download/) is a free and open-source software for enabling anonymous communication by directing Internet traffic through a free, worldwide, volunteer overlay network consisting of more than seven thousand relays.
  In short it is very slow, but it is free and it is secure. It's close to impossible to censor the Tor Browser, it is a very good choice for those wanting to use a VPN just to browse a website or two that may be geolocked. A video on how onion routing works (what the Tor Browser does) can be found [here](https://www.youtube.com/watch?v=QRYzre4bf7I), a simplified video can be found [here](https://www.youtube.com/watch?v=wlP1JrfvUo0). [ Bittorrent over Tor isn't a good idea, use a VPN for that](https://blog.torproject.org/bittorrent-over-tor-isnt-good-idea)

---
### Brave, Opera / Opera GX, Vivaldi

#### Brave

* The whole business idea of Brave from the start is to have shady [affiliate links](https://www.theverge.com/2020/6/8/21283769/brave-browser-affiliate-links-crypto-privacy-ceo-apology) and [replace ads on websites with their own](https://www.wired.com/2016/04/brave-software-publishers-respond)
* Then comes the fact that they claim they block Facebook, Twitter Trackers, yet despite this claim, [Brave actually disables its tracking protections for Facebook and Twitter's spyware scripts that allow them to track people across the web](https://www.bleepingcomputer.com/news/security/facebook-twitter-trackers-whitelisted-by-brave-browser).
  Brave's spyware protections, and any claims that it makes to work in the interests of its users, cannot be taken seriously. Brave is actively working against its users while lying to them about supposed privacy protections that it offers.
* Their security team is a joke, they have left leaks in their Android app [where websites would know detailed information about your device for almost two years](https://github.com/brave/brave-browser/issues/7758).
  And have also left unpatched [WebRTC exploits that could reveal your IP address when using a VPN for YEARS](https://web.archive.org/web/20200514123035/https://github.com/brave/browser-ios/issues/1148),
  before you [couldn't even completely disable WebRTC](https://github.com/brave/brave-browser/issues/551), and these leaking issues still plague the community to this day.
* While running, [Brave collects telemetry that is opt-out, instead of opt-in.](https://web.archive.org/web/20201229081726/https://brave.com/privacy-preserving-product-analytics-p3a/)
* Brave has made [false claims about uBlock Origin being slower than Brave's built in adblocker](https://github.com/gorhill/uBlock/issues/1279)
* Brave has [taken money on behalf of YouTubers without any consent or knowledge from the person involved.](https://web.archive.org/web/20181221180137/https://twitter.com/tomscott/status/1076160882873380870).
  The funds taken from people donating (which thought they were donating to a creator) never received the rightful person who should have received it.

#### Opera / Opera GX

* [They collect your name, IP-address, location, non-personal technical data (such as manufacturer, screen resolution, phone region if applicable)](https://www.opera.com/privacy).
  This data is associated with a unique ID that is used to distribute to third-parties, which may monitor traffic (including searches).
* [Sold to a Chinese consortium for $600 million](https://www.engadget.com/2016-07-18-opera-browser-sold-to-a-chinese-consortium-for-600-million.html)
* As for Opera VPN, there is no such thing as a free VPN, [see free VPN section.](https://github.com/CommandMC/24HS-Wiki/blob/main/productstoavoid.md#any-and-all-free-vpns)
* [Opera offered predatory loans by deploying in their apps "bait and switch" tactics to lure borrowers and charge extortionate interest rates of up to 438%](https://www.androidcentral.com/opera-accused-offering-predatory-loan-apps-interest-rates-above-300)
* Every single time you visit a site using Opera, [information is sent to to Opera on what you visited](https://spyware.neocities.org/images/opera_sitecheck.png)
* [Your geolocation is sent to Opera](https://spyware.neocities.org/images/opera_geo.png). [It also makes requests to Cxense analytics, which is a company that assigns you a unique ID to help sell you ads](https://www.cxense.com/about-us).
  Opera makes [millions off selling their users data](https://investor.opera.com/news-releases/news-release-details/opera-limited-announces-fourth-quarter-and-full-year-2019)
* Opera is closed source with no way to audit the browser. They also have publicly stated [they do not intend to reveal their source code](https://web.archive.org/web/20131104092810/http://www.operasoftware.com/press/faq/).

#### Vivaldi

* Vivaldi is [Proprietary Freeware](https://vivaldi.com/privacy/vivaldi-end-user-license-agreement/), while they claim that that [most of the code in the browser is from open source projects](https://vivaldi.com/blog/vivaldi-browser-open-source/),
  we have no way to prove that since [Vivaldi builds are not reproducible, unlike those from Firefox](https://tests.reproducible-builds.org/debian/bullseye/amd64/index_reproducible.html)
* From [Vivaldi's privacy policy](https://vivaldi.com/privacy/browser/): "When you install Vivaldi browser ('Vivaldi'), each installation profile is assigned a unique user ID that is stored on your computer.
  Vivaldi will send a message using HTTPS directly to our servers located in Iceland every 24 hours containing this ID, version, CPU architecture, screen resolution and time since last message."
  This has been confirmed by the [now deleted forum post of users seeing Piwik collecting data and sending it to third parties (domains which are not confirmed to be of Vivaldi)](https://web.archive.org/web/20180214185847if_/https://forum.vivaldi.net/topic/24029/return-of-vivaldi-spyware)

#### Recommended alternatives

* There is **no reason to use Brave/Opera/Vivaldi.** If using a Chromium browser is not a requirement, [Firefox](https://www.mozilla.org/en-US/firefox) is a solid choice.
* If you wish to use a Chromium browser that is open source, [Ungoogled chromium](https://github.com/Eloston/ungoogled-chromium) is for you.
  Want the extensions from the Google extension store? Takes [a minute to install an extension](https://ungoogled-software.github.io/ungoogled-chromium-wiki/faq#can-i-install-extensions-or-themes-from-the-chrome-webstore)
  then another second to allow it to [auto update said extensions](https://ungoogled-software.github.io/ungoogled-chromium-wiki/faq#will-extensions-auto-update)
* For VPN recommendations, see the [free VPN section](https://github.com/CommandMC/24HS-Wiki/blob/main/productstoavoid.md#any-and-all-free-vpns).

---
### Multiple AV software
#### Kaspersky

* Kaspersky is Russian company and worked for Russian government in the past. While it is not likely to be used as spyware itself, theoretically there could be made exceptions for malware in the database by request of their government. They would have to comply. What is worse, they might keep it silent.
* While there is no hard evidence of any back doors in their software or any ties to the Russian mafia or state... [but there is still a concern that you can’t operate in Russia without being controlled by the ruling party](https://www.nytimes.com/2012/06/04/technology/cyberweapon-warning-from-kaspersky-a-computer-security-expert.html?pagewanted=all)
* [These concerns have pushed the U.S Government to ban Kaspersky software in federal agencies](https://www.washingtonpost.com/world/national-security/us-to-ban-use-of-kaspersky-software-in-federal-agencies-amid-concerns-of-russian-espionage/2017/09/13/36b717d0-989e-11e7-82e4-f1076f6d6152_story.html)
* [In August 2015, Bloomberg News reported that Kaspersky Lab changed course in 2012, as "high-level managers have left or been fired, their jobs often filled by people with closer ties to Russia's military or intelligence services. Some of these people actively aid criminal investigations by the FSB, the KGB’s successor, using data from some of the 400 million customers](https://www.bloomberg.com/news/articles/2015-03-19/cybersecurity-kaspersky-has-close-ties-to-russian-spies)

If the US government doesn't trust a specific software, neither should you.

#### Avast

* Leaked documents have shown that they sell [**'Every search. Every click. Every buy. On every site.**](https://www.vice.com/en_us/article/qjdkq7/avast-antivirus-sells-user-browsing-data-investigation)
* They have injected users [with adware to sell your data while browsing](https://www.howtogeek.com/199829/avast-antivirus-was-spying-on-you-with-adware-until-this-week).
* [Subsidiaries has cooperated in handing over customer data which was supposed not to be gathered](https://yro.slashdot.org/story/11/09/25/0415213/hidemyasscom-doesnt-hide-logs-from-the-fbi)

#### Norton

* Norton is criticized due to refusing to [uninstall completely](https://web.archive.org/web/20090221124023/http://www.askdavetaylor.com/how_can_i_fully_remove_norton_antivirus_from_my_system.html), eventually requiring [to create a dedicated tool to uninstall it completely](https://web.archive.org/web/20090223150611/http://service1.symantec.com/Support/tsgeninfo.nsf/docid/2005033108162039)
* [Whitelisted keylogger intended to obtain passwords to encrypted e-mails and other documents during investigations](https://en.wikipedia.org/wiki/Norton_AntiVirus#FBI_cooperation)

#### Recommended alternatives

* [Malwarebytes](https://www.malwarebytes.com), ranks well on [av-comparatives.org](https://www.av-test.org/en/antivirus/home-windows/windows-10/august-2020/malwarebytes-premium-4.1.2-203116)
* [ESET](https://www.eset.com/us), ranks on [av-comparatives.org](https://av-comparatives.org) among the top players.
* [Windows Defender](https://www.microsoft.com/en-us/windows/comprehensive-security) plus common sense! These days the best anti-virus is not installing from unknown sources (never whitelist an .exe just because someone tells you to!). Rarely can something infect you from your browser (assuming it is up to date and not compromised). Stay [up to date](https://old.reddit.com/r/24hoursupport/wiki/systemuptodate), don't install from unknown sources, and use your judgement.

---
### Apple

* This is a vast topic to cover, the majority of it is covered here: https://stallman.org/apple.html
* Apple [lobbies against bill meant to prevent slave labor](https://web.archive.org/web/20201122061805/https://www.washingtonpost.com/technology/2020/11/20/apple-uighur/)
* [Apple uses spite to force planned obsolescence](https://www.youtube.com/watch?v=NVAmnV65_zw)
* They can't design a product correctly. The majority of their products from the beginning have had issues, from their MacBooks to their iPhones. They also unnecessarily do things in the name of "security",
  such as gluing in batteries to iPhones, using non-standard screws, SOLDERING IN RAM STICKS, list goes on. 
  
  For more info, watch this video: https://www.youtube.com/watch?v=AUaJ8pDlxi8

* They overcharge massively for underspecced products. For example, you can spend 1200 dollars on an iMac, and you will get a 5400rpm drive with no SSD in that machine. Here's an example of what 1439 dollars will get you as of December 2020 should you choose to build your own PC: https://pcpartpicker.com/list/rNDrYg
  
  Compare this to a 1300 dollar iMac: https://www.apple.com/shop/buy-mac/imac
  
  For about 130 dollars more, you get double the memory capacity with much higher speeds, a SIGNIFICANTLY better CPU AND GPU, far more storage, and a high refresh rate 1080p IPS monitor.
  Granted, the iMac is a 4K monitor, but it's only 21.5" and at that small of a screen size, 4K doesn't look great natively on such a small screen. You are getting A LOT more bang for your buck with that PC as an example.
  
  Best part is, if something breaks, you can send it in for RMA or potentially fix it yourself! You cannot do such a thing with Apple products without special tools or going to a Genius Bar or a 3rd party repair shop.

* They overcharge for repairs or blatantly misdiagnose issues before charging you insane amounts of money to "fix" them as a way to bully you into buying a new product: https://www.youtube.com/watch?v=o2_SZ4tfLns
* They also have repeatedly lobbied against Right to Repair, which is a bill that allows 3rd party repair business to work on various products from various companies without fear of reprisal from whatever company sold said product from phones to cars to tractors: https://www.nytimes.com/2020/10/23/climate/right-to-repair.html

---
### Ubuntu / Ubuntu derivatives 

#### Security

* The main issue with "backporting" fixes to older versions is two main parts. First one is that Canonical doesn't audit every single package they are leaving out of date, which has resulted in multiple scenarios where security issues that have been fixed in previous releases were left unpatched, [like with VLC where an issue was patched 16 months ago before it was discovered](https://twitter.com/videolan/status/1153963312981389312).
  If Ubuntu had updated the dependencies VLC depends on, they would have never been vulnerable to the exploit.
* Canonical backports security fixes that get assigned a CVE, [but security *improvements* don't get backported](https://outflux.net/blog/archives/2021/02/08/security-things-in-linux-v5-8/).
  Not only do they ignore issues with the most important package (the kernel), but they constantly leave security issues that require updates in popular applications like [qbittorrent](https://ubuntu.com/security/cve?q=&package=qbittorrent&priority=&version=&status=),
  [rclone](https://ubuntu.com/security/CVE-2020-28924), and [a lot and A LOT AND A LOT MORE](https://ubuntu.com/security/cve?version=current&offset=0) that could simply be solved by just [UPDATING!](https://security.archlinux.org/).
* Because of the nature of updates, the development team of software will focus on the **latest version** of it unless they offer an LTS branch. They aren't going to waste time and resources maintaining older releases,
  most security backfixes that end up in older packages on Ubuntu are security issues that were found on newer releases that happened to affect older releases aswell, often times [there are issues in older releases that do not exist in newer releases of the software](https://news.ycombinator.com/item?id=23616150),
  this is why maintaining older packages requires a lot more development resources.

#### PPAs are not the solution to any of these problems

* Despite popular belief, having one part of the system be up to date then the rest out of date is not a situation you want to be in. Not to mention PPAs defeat the entire reason you're supposedly using Ubuntu, for "stability", sadly this is a misconception.
  While it is true that workloads that depend on / benefit from no change would increase stability, unchanging **does not mean stability**. You can have updates for your system and still have it be stable. **Delaying updates indefinitely is not the solution to an issue you're having**.

#### Recommended alternatives

* [Fedora](https://getfedora.org/) is a Linux distribution developed by the Fedora Project and sponsored by Red Hat. Fedora Workstation is a secure, reliable, and UP TO DATE developed for desktops and laptops (hence not for servers or enterprise workspaces, unlike Ubuntu).
  Fedora by default comes with the GNOME desktop environment, [a lot of other desktop environments (like KDE) are also available.](https://spins.fedoraproject.org/)

---
### Manjaro

* This is a vast topic to cover, the majority of it is covered here: https://manjarno.snorlax.sh/

#### Security

* SSL Certificates: Manjaro has let their certificates expire 5 Times.
* Holding back packages for 2 weeks can also cause security issues.

#### Stability

* Arch is overall more stable than Manjaro and even though they hold back packages for 2 weeks it doesnt make it any more stable just means updates reach you later and ends up casing more issues

##### The AUR
* This is better Explained at https://manjarno.snorlax.sh/ but summed up AUR scripts are user made meaning you should look through them before running them and most of these scripts are written with the assumption that you aren’t running a system that’s effectively two weeks out of date. This causes [Partial Upgrades](https://wiki.archlinux.org/title/System_maintenance#Partial_upgrades_are_unsupported) At best, that program won’t install or work correctly and at worst can cause all kinds of issues on your system with no obvious way to fix it. And that they don't actually support the AUR, They just blame the users of pamac. They also provide insufficient warnings about the AUR and the potential risks, while providing a simplified interface for installing AUR packages via pamac.

##### Rushing Asahi out the door
In their attempt to get Asahi Linux out (and support Apple Silicon) as soon as possible, they ended [pulling the latest PKGBUILD without talking to the devs](https://web.archive.org/web/20221208084616/https://twitter.com/marcan42/status/1576414477272387584). This has resulted in them shipping potentially broken kernels to end users.

Still though, that’s besides the main problem. It was [only about 3 days ago this video came out](https://www.youtube.com/watch?v=k0cnMUroMlQ), in which a DE is working for the first time. Not only is it still in a state far from prime-time, but compounded with the tweet above they didn’t even bother trying to speak with the devs of the project about its current state.

#### Management

##### Funding

Manjaro has had a controversy with their treasurer. Phillip Muller (Manjaro team lead) had purchased a laptop for €2000, and the treasurer asked to clarify his purchase. [This ultimately led to the treasurer being removed](https://redd.it/hxp3zi). Isn’t the whole point of a treasurer to ensure fair and efficient use of donation funds?

#### Poor QA

##### DDoSing the AUR

Manjaro’s AUR helper, pamac, shipped a version with a bug on 2020-04-26 that accidentally sent thousands of requests to the AUR per user. This rendered the AUR offline for all users across every Arch-based distro for a few hours.

* https://www.reddit.com/r/archlinux/comments/mz3biz/is_the_aur_down_for_everyone/
* https://gitlab.manjaro.org/applications/pamac/-/issues/1017

##### and again...

On 2021-10-14, Manjaro once again shipped a bad version of pamac, resulting in pamac being blocked again. This may have been the cause for the day’s earlier outage.

* https://www.reddit.com/r/linux/comments/q85t8n/pamac_manjaros_package_manager_gui_has_been/

* https://gitlab.manjaro.org/applications/pamac/-/issues/1135

While these incidents were in no way intentional, it highlights the poor QA testing that Manjaro performs. This has happened on two separate occasions in less than two years.

#### Miscellaneous

[Their system update script used to run rm on the lockfile mid-transaction](https://gitlab.manjaro.org/packages/core/manjaro-system/blob/3b806753e245b7ec7e18bb674e916e28d751a429/manjaro-update-system.sh#L45). The lockfile is in place to prevent multiple instances of pacman from trying to alter the package database at the same time. Sometimes, when pacman is interrupted, a stale lockfile can remain. In this case, removing the lockfile is a common troubleshooting step. However, you should only do that when you are absolutely certain there are no other pacman instances running. Manjaro’s script used to do this silently without checking for other instances.

#### Recommended alternatives

* Arch [and it already has a installer](https://github.com/archlinux/archinstall)

* [EndeavourOS](https://endeavouros.com/) seems to be what Manjaro is going for – just rightly done as far as I can tell. That said, using an Arch derivative is still a bit questionable in my view. The main excuse for doing so (lack of an automated installer) doesn’t apply anymore as Arch ships with archinstall. However, EndeavourOS has a GUI installer, which should be much more approachable, and offers many more configurations to choose from out of the box than archinstall.

Once again though, I’d like to reiterate that Arch already ships with a reasonably friendly installer.

---
### Windows 7

#### Security

Windows 7 is an end of life (EOL) operating system, meaning the makers (Microsoft) are no longer supporting it, this means we will also offer no support for this operating system.
This is due to issues with EOL operating systems being most definitely caused by it no longer receiving any sort of support from anyone. 
Running any EOL OS, not just Windows 7, is very dangerous. Not only will manufacturers stop providing driver support for new and already existing components, making the stability problem worse,
but you will also stop receiving security updates. No software can protect you from issues that come from the operating system itself.

All these issues result in a very unstable situation that has no fix besides getting on a properly supported operating system, which means we will only offer support for you with updating to a properly supported operating system. 

#### Privacy concerns

If you are staying on Windows 7 due to of privacy concerns, understand you **cannot have privacy without security**. What is the point of Microsoft not knowing what you do but everyone and their dog knows? 

If you want to use a privacy-respecting OS, use Linux instead (see below for recommendations).  
Note: Modifying Windows to not send analytics data is **not supported**, if you modified Windows, our only advice will be to reinstall

#### Performance concerns

If you are staying on Windows 7 due to performance concerns, do try Windows 10 and see if it works.
While some old hardware may just not be able to handle it, Windows 10 does bring optimizations that do improve performance. Alternatively you can use one of the recommended Linux distros below.

#### Recommended alternatives

* Windows 10 is the most logical choice for most users, guide on how to clean install can be found [here](https://github.com/CommandMC/24HS-Wiki/blob/main/installingwindows.md)
* Fedora is likely the second choice for most if you do not have Nvidia hardware, you can run Windows applications on Fedora [following this guide](https://computingforgeeks.com/how-to-install-wine-on-fedora/), you can also check and see if your [games work on Linux](https://www.protondb.com/).
  The Fedora ISO [can be found here](https://spins.fedoraproject.org/kde/), instructions on how to install can be found below

Download the ISO above, download and install [Etcher](https://www.balena.io/etcher/).
Run Etcher, click "Flash from file" then select the ISO you downloaded. Then select target as the USB (**make sure it is empty, everything on it will be deleted**) and finally click flash.
Once this is done you [go to BIOS and set the boot priority to the USB](https://github.com/CommandMC/24HS-Wiki/blob/main/enteringbios.md), boot into the USB, and the installation process from there is mostly straightforward.
