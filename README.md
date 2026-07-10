# Cyber-Security-All-Information


Skip to content
Navigation Menu
Platform
Solutions
Resources
Open Source
Enterprise
Pricing

Search or jump to...
Sign in
Sign up
 You signed in with another tab or window. Reload to refresh your session.
rawfilejson
/
awesome-osint-arsenal
Public
Code
Issues
2
Pull requests
6
Actions
Projects
Security and quality
Insights
rawfilejson/awesome-osint-arsenal
Go to file
Name		
author
rawfilejson
Merge branch 'main' of https://github.com/rawfilejson/awesome-osint-a…
1f1accb
 · 
2 months ago
assets
Delete assets/logo.jpg
2 months ago
README.md
Update Xquik link to point to GitHub homepage
2 months ago
blueteam.sh
update
2 months ago
extras.sh
update
2 months ago
forensics.sh
update
2 months ago
hardware.sh
update
2 months ago
install.sh
update
2 months ago
labs.sh
update
2 months ago
osint.sh
update
2 months ago
redteam.sh
update
2 months ago
termux.sh
update
2 months ago
tools.json
Version 2.1
2 months ago
Repository files navigation
README
OSINT Arsenal
🔍 AWESOME OSINT ARSENAL
The Ultimate Open-Source Intelligence + Security Toolkit

Tools Categories Version Updated Stars


751+ tools · 50 categories · Multi-distro installers · Georgian OSINT · Termux support

The most comprehensive OSINT and security toolkit on the internet — every tool with installation instructions or a verified link.

Buy Me a Coffee


⚡ Get everything in one command
git clone https://github.com/rawfilejson/awesome-osint-arsenal && cd awesome-osint-arsenal && sudo bash install.sh
🎯 Or pick just what you need
sudo bash osint.sh        # 🔍 OSINT only (Sherlock, Maigret, Amass, …)
sudo bash redteam.sh      # ⚔️  Red team (Sliver, BloodHound, Mimikatz, Nuclei, …)
sudo bash blueteam.sh     # 🛡️  Blue team (Wazuh, Sigma, Suricata, Velociraptor, …)
sudo bash forensics.sh    # 🔬 DFIR + RE (Volatility, Ghidra, radare2, …)
sudo bash hardware.sh     # 🔌 Hardware + SDR (binwalk, hackrf, openocd, …)
sudo bash labs.sh         # 🎓 Vulnerable apps for practice (DVWA, Juice Shop, …)
bash termux.sh            # 📱 Android (Termux subset, no sudo needed)
Works on Kali, Debian, Ubuntu, Parrot, Mint, Pop!_OS (best — apt) Partial on Arch / Manjaro / Fedora / RHEL (auto-detected, falls back to git/pip/go) Termux subset on Android


Important

🙏 A note before you fork
This repo has 751 tools across 50 categories. Keeping that current — links, install commands, new tools every week — is a lot for one person.

If nobody helps, parts of this list will go stale. That's just real talk.

How you can help in 30 seconds:

⭐ Star the repo (more stars = more contributors find it)
🐛 Spotted a dead link? Open an issue, takes 1 minute
☕ Buy me a coffee so weekends keep going to this
📢 Share it — tweet, Discord, wherever the security crowd hangs out
If something's broken: don't just complain — open an issue or PR. That's how this stays useful.

Warning

DISCLAIMER: This repository is for educational and authorized security research only. Always obtain written permission before testing systems you do not own. The authors are not responsible for any misuse of the tools or techniques listed here. See the full Legal Disclaimer at the bottom.

📋 Table of Contents
🔭 Reconnaissance & Discovery — click to expand
💥 Data Breaches & Leaks — click to expand
🕶️ Dark Web & Privacy — click to expand
⚔️ Offensive Security (Authorized Testing Only) — click to expand
🧠 Intelligence & Analysis — click to expand
👁️ Surveillance & Dorking — click to expand
🌐 Community & Platforms — click to expand
🧰 Toolkits & Frameworks — click to expand
🖥️ Hardware & Operating Systems — click to expand
👨‍💻 Developer & Learning — click to expand
⚡ Quick Reference — click to expand
⚔️ Red Team & Blue Team — click to expand
🔬 Forensics, Hardware & Training — click to expand
📚 Knowledge & Curated Additions — click to expand
🇬🇪 Country-Specific OSINT — click to expand
⚙️ Installation Guide
Quick install — Kali / Debian / Ubuntu / Parrot
git clone https://github.com/rawfilejson/awesome-osint-arsenal
cd awesome-osint-arsenal
sudo bash install.sh
Pick a single stack
Script	What it installs	Use when
osint.sh	OSINT tools (Sherlock, Maigret, Amass, theHarvester, …)	You only do recon / investigations
redteam.sh	Sliver, BloodHound, Impacket, NetExec, Mimikatz, Nuclei, …	Authorized pentesting / red team
blueteam.sh	Wazuh, Sigma, Suricata, Velociraptor, Atomic Red Team, MITRE CALDERA	SOC / detection engineering
forensics.sh	Volatility 3, Ghidra, radare2, Plaso, CyberChef, …	DFIR / malware analysis
hardware.sh	binwalk, hackrf, openocd, GNU Radio, gqrx, …	RF / IoT / firmware research
labs.sh	DVWA, Juice Shop, WebGoat (Docker)	Local practice labs
termux.sh	Android-compatible subset	Phone-based recon
Other Linux distros
The installers auto-detect your package manager:

Distro	Manager	Status
Kali / Debian / Ubuntu / Parrot / Mint / Pop!_OS	apt	✅ Best — primary target
Arch / Manjaro / EndeavourOS	pacman	🟡 Partial (apt-only tools skip cleanly)
Fedora / RHEL / Rocky / Alma	dnf	🟡 Partial (apt-only tools skip cleanly)
Termux (Android)	pkg	✅ Subset only — use bash termux.sh
macOS / Windows	—	❌ Use a Kali VM or WSL2
What every installer does
Detects your distro and uses the right package manager
Skips what's already installed (idempotent — safe to re-run)
Color output: 🟢 installed · 🟡 skipped · 🔴 failed
Logs failures to ~/osint-install-errors.log
Prints a summary at the end
Tools cloned via git go to /opt/osint-arsenal/ (or $HOME/osint-arsenal/ on Termux)
After install — add tools to your PATH
echo 'export PATH="$PATH:/opt/osint-arsenal"' >> ~/.bashrc
source ~/.bashrc
Tools installed via apt/pip/go install are already on your $PATH.

📊 Stats at a Glance
🛠️ Total Tools	💻 CLI Tools	📁 GitHub Repos	🌐 Online Platforms	🤖 AI Tools
751+	165+	117+	461+	25+
🕶️ Dark Web	🇬🇪 Georgian OSINT	💥 Breach Engines	⚔️ Red Team	🛡️ Blue Team
15+	500+	39+	35+	24+
🔬 Forensics	🔌 Hardware	🎓 Training	🎯 Bug Bounty	📂 Total Categories
16+	16+	21+	12+	50
Buy Me a Coffee

1. Username & Social Media OSINT
🎯 Find accounts, profiles, and digital footprints across hundreds of platforms.

Pro tip: Start with Sherlock for a quick sweep, then use Maigret for depth — it covers 3000+ sites.

Tool	Description	Install / Link
Sherlock	Find usernames across 400+ social networks	pip install sherlock-project
Maigret	Advanced Sherlock fork — 3000+ sites	pip install maigret
Namechk	Username & domain availability checker	namechk.com
WhatsMyName	Web-based username enumeration	whatsmyname.app
Snoop	Username search (Russian-focused)	pip install snoop
UserRecon	Bash-based username finder	git clone https://github.com/wishihab/userrecon.git
Blackbird	Fast username search tool	pip install blackbird-osint
Social Analyzer	API-based social media profiler	pip install social-analyzer
NExfil	Find profiles by username	pip install nexfil
Socid-extractor	Extract info from web pages	pip install socid-extractor
Gitrecon	GitHub OSINT reconnaissance	pip install gitrecon
OSRFramework	Username research framework	pip install osrframework
Holehe	Check if email is registered on 120+ sites	pip install holehe
socialscan	Check email/username availability	pip install socialscan
Investigo	Username checker (Go-based)	go install github.com/tdh8316/investigo@latest
OSINT Framework	Visual map of all OSINT tools	osintframework.com
CheckUserNames	Check username across multiple platforms	checkusernames.com
KnowEm	Username search on 500+ sites	knowem.com
Instant Username Search	Real-time username checker	instantusername.com
Usersearch.org	Free social network search	usersearch.org
💻 Sherlock — Install & Usage
💻 Maigret — Install & Usage
2. Email OSINT Tools
📧 Verify emails, find linked accounts, check breach exposure, and analyze headers.

Pro tip: Holehe is free and fast. h8mail is best for breach correlation when API keys are configured.

Tool	Description	Install / Link
h8mail	Email OSINT & breach hunting	pip install h8mail
Holehe	Check email on 120+ sites	pip install holehe
theHarvester	Email & domain harvester	pip install theHarvester
EmailAnalyzer	Analyze suspicious .eml files	git clone https://github.com/keraattin/EmailAnalyzer
Prowl	Email & domain reconnaissance	git clone https://github.com/nettitude/Prowl
EmailHeader-Analyzer	CLI email header parser + OSINT	git clone https://github.com/Giritharram/EmailHeader-Analyzer-CLI-Python
MailHeaderDetective	Email header forensics	git clone https://github.com/akajhon/MailHeaderDetective
WhatMail	Email header analysis CLI	git clone https://github.com/z0m31en7/WhatMail
mailto_analyzer	Email exposure analysis	pip install mailto-analyzer
Infoga	Email OSINT gathering	git clone https://github.com/m4ll0k/Infoga
Hunter.io	Find professional emails	hunter.io
Phonebook.cz	Email, domain & URL search	phonebook.cz
EmailRep	Email reputation lookup	emailrep.io
Epieos	Get info linked to email	epieos.com
GetNotify	Email open tracking + geolocation	getnotify.com
Snov.io	Email finder & verifier	snov.io
MXToolbox	Email header analysis & DNS checks	mxtoolbox.com
SimpleLogin	Email alias service for OSINT	simplelogin.io
Email-Checker	Email validation tool	email-checker.net
Voila Norbert	Find anyone's email	voilanorbert.com
💻 h8mail — Install & Usage
3. Phone Number OSINT
📱 Identify carriers, locations, registrations, and linked accounts from phone numbers.

Pro tip: PhoneInfoga is the gold standard CLI tool. GetContact reveals how a number is saved by others.

Tool	Description	Install / Link
PhoneInfoga	Advanced phone number scanner	pip install phoneinfoga
Ignorant	Check phone registrations on sites	pip install ignorant
GetContact	See how number is saved by others	getcontact.com
NumVerify	Phone number validation API	numverify.com
Truecaller	Caller ID & spam lookup	truecaller.com
Sync.me	Phone number lookup	sync.me
CallerIDTest	Reverse phone lookup	calleridtest.com
SpyDialer	Free reverse phone lookup	spydialer.com
National Cellular Directory	Phone owner lookup	nationalcellulardirectory.com
TelPoisk	Russian phone directory	telpoisk.com
NumLookup	Free reverse phone lookup	numlookup.com
Hlr-Lookups	HLR phone number lookup	hlr-lookups.com
PhoneSploit	ADB-based phone exploitation	git clone https://github.com/aerosol-can/PhoneSploit
💻 PhoneInfoga — Install & Usage
4. Domain & IP OSINT
🌐 Enumerate subdomains, query DNS records, discover IP ranges, and map attack surfaces.

Pro tip: Run amass + subfinder together for maximum subdomain coverage, then pipe into httpx to check which hosts are live.

Tool	Description	Install / Link
Amass	In-depth DNS enumeration	go install github.com/owasp-amass/amass/v4/...@master
Subfinder	Fast passive subdomain discovery	go install github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
dnsrecon	DNS enumeration	pip install dnsrecon
Sublist3r	Subdomain enumeration	pip install sublist3r
crt.sh	Certificate transparency search	crt.sh
Shodan	Internet-connected device search	shodan.io
Censys	Internet-wide scan search	censys.io
Criminal IP	AI-powered cyber threat intelligence	criminalip.io
VirusTotal	Domain/IP/file analysis	virustotal.com
SecurityTrails	DNS & domain intelligence	securitytrails.com
IPGeoLocation	IP address geolocation	git clone https://github.com/maldevel/IPGeoLocation
Nmap	Network scanner & mapper	apt install nmap
Masscan	Fastest internet port scanner	apt install masscan
WHOIS.com	WHOIS domain lookup	whois.com
ViewDNS	Multiple DNS tools	viewdns.info
DNSDumpster	DNS reconnaissance & mapping	dnsdumpster.com
Robtex	DNS lookup visualization	robtex.com
ARIN WHOIS	IP registration database	whois.arin.net
BGP Toolkit	BGP/ASN/IP intelligence	bgp.he.net
urlscan.io	URL/domain analysis & screenshots	urlscan.io
AbuseIPDB	IP address reputation database	abuseipdb.com
Web-Check	All-in-one website analysis	web-check.xyz
IPinfo	IP address data & geolocation	ipinfo.io
DB-IP	IP geolocation database	db-ip.com
💻 Amass + Subfinder + HTTPx — Most effective recon combo
5. Geolocation & Maps OSINT
🗺️ Geolocate images, analyze satellite data, and verify photo locations.

Pro tip: Combine SunCalc (shadow analysis) + ShadowMap + Mapillary for precision image geolocation.

Tool	Description	Link
Google Earth Pro	Advanced satellite imagery	earth.google.com
Overpass Turbo	OpenStreetMap data query	overpass-turbo.eu
SunCalc	Sun position/time calculator from photos	suncalc.org
GeoGuessr	Geolocation training game	geoguessr.com
Sentinel Hub	Satellite imagery access	sentinel-hub.com
FIRMS	NASA fire/thermal hotspots	firms.modaps.eosdis.nasa.gov
Wikimapia	Collaborative world map	wikimapia.org
OpenStreetMap	Free world map	openstreetmap.org
GeoSpy	AI-powered image geolocation	geospy.ai
Mapillary	Street-level imagery	mapillary.com
Maxar	Commercial satellite imagery	maxar.com
F4map	3D interactive world map	demo.f4map.com
Zoom Earth	Real-time satellite & weather	zoom.earth
KartaView	Street-level imagery (OpenStreetCam)	kartaview.org
ShadowMap	Shadow analysis for time estimation	shadowmap.org
Crime Brasil	Brazil crime + accidents open data by neighborhood (bairro-level RS; municipal MG/RJ; PRF accidents)	crimebrasil.com.br
6. Image & Video OSINT
🖼️ Extract metadata, reverse search images, verify authenticity, and detect AI-generated content.

Pro tip: Yandex reverse image search consistently outperforms Google for finding faces and locations.

Tool	Description	Install / Link
TinEye	Reverse image search	tineye.com
Google Reverse Image	Google image search	images.google.com
Yandex Images	Best reverse image search for faces/places	yandex.com/images
ExifTool	Image/document metadata extraction	apt install libimage-exiftool-perl
FOCA	Metadata extraction from documents	github.com/ElevenPaths/FOCA
InVID	Video verification toolkit	invid-project.eu
FotoForensics	Image forensic analysis (ELA)	fotoforensics.com
Fake Image Detector	AI-based fake image detection	fakeimagedetector.com
Search by Image	Multi-engine reverse image (browser ext)	Chrome / Firefox extension
Depix	Recover pixelated text from screenshots	git clone https://github.com/beurtschipper/Depix
Forensically	Online image forensics suite	29a.ch/photo-forensics
AI or Not	Detect AI-generated images	aiornot.com
Hive Moderation	AI content detection	hivemoderation.com
Illuminarty	AI image detection	illuminarty.ai
💻 ExifTool — Install & Usage
7. Facial Recognition & People Search
👤 Find people across the web using photos, names, or usernames.

⚠️ Warning: Facial recognition has serious privacy and legal implications. Use only with explicit authorization.

Tool	Description	Install / Link
FaceSeek	AI-powered reverse face search	faceseek.online
FaceCheck.ID	Face recognition search engine	facecheck.id
PimEyes	Face search engine from photos	pimeyes.com
Search4faces	Face search in VK/OK social networks	search4faces.com
face_recognition	Python face recognition library	pip install face_recognition
DeepFace	AI face analysis (age, gender, emotion)	pip install deepface
ThatsThem	Free people search	thatsthem.com
Pipl	Deep people search engine	pipl.com
BeenVerified	People search & background check	beenverified.com
Spokeo	People search aggregator	spokeo.com
FastPeopleSearch	Free people finder	fastpeoplesearch.com
WebMii	People search engine	webmii.com
OSINT Industries	People search + social media lookup	osint.industries
IDCrawl	Free people search engine	idcrawl.com
8. Social Media Monitoring
📡 Monitor, scrape, and investigate social media accounts and communities.

Pro tip: Combine Osintgram (Instagram) + Telepathy (Telegram) + snscrape (Twitter/X) for full platform coverage.

Tool	Description	Install / Link
Osintgram	Instagram OSINT tool	git clone https://github.com/Datalux/Osintgram
Instaloader	Instagram data downloader	pip install instaloader
Twint	Twitter OSINT (no API needed)	pip install twint
snscrape	Social media scraper (Twitter, Reddit, etc.)	pip install snscrape
Toutatis	Instagram OSINT by phone/email	pip install toutatis
TikTok Scraper	TikTok data extraction	npm install -g tiktok-scraper
Reddit Investigator	Reddit user analysis	reddit-user-analyser.netlify.app
socialscan	Social media presence checker	pip install socialscan
Telepathy	Telegram OSINT analysis	pip install telepathy
Twayback	Find deleted tweets	pip install twayback
Xquik	X/Twitter data API & MCP skill	github.com
SocialBlade	Social media analytics	socialblade.com
Social-Searcher	Free social media search engine	social-searcher.com
Mention	Social media monitoring	mention.com
BrandWatch	Social listening platform	brandwatch.com
9. Data Breach & Leak Search Engines
💥 Check if credentials, emails, or phones have been exposed in data breaches.

Pro tip: HIBP is free and safe. DeHashed and LeakCheck offer the most data for paid tiers.

Tool	Description	Type	Link
Have I Been Pwned	Check email/phone in breaches	🟢 Free	haveibeenpwned.com
DeHashed	Breach search engine	💰 Paid	dehashed.com
LeakCheck	Email/username/phone breach search	🟡 Freemium	leakcheck.net
Intelligence X	Search breaches, darknet, leaks	💰 Paid	intelx.io
BreachDirectory	Free breach search	🟢 Free	breachdirectory.org
LeakPeek	Search leaked databases	🟡 Freemium	leakpeek.com
Snusbase	Breach data search engine	💰 Paid	snusbase.com
CheckLeaked	Leak search engine (15B+ accounts)	🟡 Freemium	checkleaked.cc
DataBreach.com	Data breach lookup	🟢 Free	databreach.com
Hudson Rock Cavalier	Infostealer intelligence & breach data	🟡 Freemium	hudsonrock.com
h8mail	Automated breach hunting CLI	🟢 Free	pip install h8mail
XposedOrNot	Breach exposure check	🟢 Free	xposedornot.com
ScatteredSecrets	Breach notification service	🟡 Freemium	scatteredsecrets.com
The OSINT Rack	Ransomware & data leak monitoring	🟢 Free	osintrack.com
Pwndb	Dark web breach database (Tor)	🟢 Free	Requires Tor Browser
OsintCat	Email, username & phone breach lookup — fast results with real data	🟡 Freemium	osintcat.net
💻 Pwndb — Dark Web Breach Search (requires Tor)
10. WikiLeaks, DDoSecrets & Whistleblower Platforms
📁 Archives of leaked government, corporate, and classified documents.

Platform	Description	Link
WikiLeaks	Leaked government & corporate documents	wikileaks.org
DDoSecrets	Distributed Denial of Secrets	ddosecrets.com
Cryptome	Documents archive since 1996	cryptome.org
The Intercept	Investigative journalism	theintercept.com
SecureDrop	Whistleblower submission system	securedrop.org
ICIJ Offshore Leaks	Panama Papers, Pandora Papers	offshoreleaks.icij.org
DocumentCloud	Public document research	documentcloud.org
Wayback Machine	Web archive	web.archive.org
FBI Vault	FBI electronic reading room	vault.fbi.gov
CIA Reading Room	Declassified CIA documents	cia.gov/readingroom
NSA Declassified	NSA declassified records	nsa.gov
PACER	US federal court records	pacer.uscourts.gov
11. Password Cracking & Credential Tools
🔑 Tools for authorized password auditing and credential recovery on systems you own.

Tool	Description	Install / Link
Hashcat	Advanced password recovery (GPU-accelerated)	apt install hashcat
John the Ripper	Classic password cracker	apt install john
Hydra	Network login brute-forcer	apt install hydra
Medusa	Parallel brute-force tool	apt install medusa
CeWL	Custom wordlist generator from website	apt install cewl
Crunch	Pattern-based wordlist generator	apt install crunch
RainbowCrack	Rainbow table cracker	project-rainbowcrack.com
Ophcrack	Windows password cracker (rainbow tables)	ophcrack.sourceforge.io
LaZagne	Credentials recovery tool (post-exploit)	git clone https://github.com/AlessandroZ/LaZagne
Mimikatz	Windows credential dumper	git clone https://github.com/gentilkiwi/mimikatz
Responder	LLMNR/NBT-NS/MDNS poisoner	git clone https://github.com/lgandx/Responder
💻 Hashcat — Quick Reference
12. Dark Web Search Engines & Tools
🕶️ Search .onion sites, darknet markets, and hidden services.

Requires: Tor Browser or Tor service running on port 9050.

Tool	Description	Link / Onion Address
Torch	Oldest & largest dark web search engine	xmh57jrknzkhv6y3ls3ubitzfqnkrwxhopf5aygthi7d6rplyvk3noyd.onion
Haystak	Dark web search with filtering	haystak5njsmn2hqkewecpaxetahtwhsbsa64jom2k22z5afxhnpxfid.onion
Ahmia	Clearnet dark web search	ahmia.fi
DuckDuckGo Onion	Private search on Tor	duckduckgogg42xjoc72x3sjasowoarfbgcmvfimaftt6twagswzczad.onion
Phobos	Dark web search engine	phobosxilamwcg75xt22id7aywkzol6q6rfl2flipcqoc4e4ahima5id.onion
DarkSearch	Dark web search API (clearnet)	darksearch.io
OnionScan	Scan & analyze .onion sites	go install github.com/s-rah/onionscan@latest
Dark.fail	Verified dark web links directory	dark.fail
OSINT-SPY	OSINT tool with Tor support	git clone https://github.com/SharadKumar97/OSINT-SPY
💻 Setting up Tor for dark web tools
13. Anonymous & Privacy Tools
🔒 Maintain anonymity during OSINT investigations and protect your identity.

Pro tip: Use Tails OS for investigations requiring full anonymity — it leaves zero trace on disk.

Tool	Description	Install / Link
Tor Browser	Anonymous web browsing	torproject.org
Tails OS	Amnesic live OS (no trace)	tails.boum.org
Whonix	Anonymous OS via Tor (VM-based)	whonix.org
ProtonVPN	Free encrypted VPN	protonvpn.com
ProtonMail	Encrypted email	proton.me
Signal	Encrypted messaging	signal.org
OnionShare	Anonymous file sharing via Tor	onionshare.org
Anonsurf	Anonymize entire OS traffic	git clone https://github.com/Und3rf10w/kali-anonsurf
MAC Changer	Change/spoof MAC address	apt install macchanger
BleachBit	Digital footprint cleaner	bleachbit.org
VeraCrypt	Disk encryption	veracrypt.fr
KeePassXC	Offline password manager	keepassxc.org
Mullvad VPN	Privacy VPN (no email needed)	mullvad.net
Anon-SMS	Anonymous SMS sending	git clone https://github.com/HACK3RY2J/Anon-SMS.git
14. Web Application OSINT & Scanning
🕸️ Fingerprint web technologies, discover hidden directories, and crawl for endpoints.

Pro tip: Run Whatweb first to fingerprint, then Nikto for quick vulns, then Nuclei for deep scanning.

Tool	Description	Install / Link
Nikto	Web server vulnerability scanner	apt install nikto
WPScan	WordPress vulnerability scanner	gem install wpscan
Wappalyzer	Technology profiler (browser ext)	Browser Extension
Whatweb	Web technology identifier	apt install whatweb
Dirb	Web directory brute-forcer	apt install dirb
Gobuster	URI/DNS brute-forcer (Go)	go install github.com/OJ/gobuster/v3@latest
Feroxbuster	Fast recursive content discovery	apt install feroxbuster
HTTPx	Fast HTTP toolkit / probing	go install github.com/projectdiscovery/httpx/cmd/httpx@latest
Katana	Web crawler	go install github.com/projectdiscovery/katana/cmd/katana@latest
LinkFinder	Discover endpoints in JavaScript	git clone https://github.com/GerbenJavado/LinkFinder
Photon	Web crawler for OSINT data	git clone https://github.com/s0md3v/Photon
Wfuzz	Web fuzzer	pip install wfuzz
ParamSpider	Parameter discovery from web archives	pip install paramspider
WebHack	Web hacking toolkit	git clone https://github.com/yan4ikyt/webhack
15. Social Engineering & Phishing
🎭 Phishing simulation frameworks for authorized red team engagements.

⚠️ For authorized penetration testing and security awareness training ONLY.

Tool	Description	Install / Link
SET (Social Engineering Toolkit)	Complete SE framework	apt install set
Gophish	Enterprise phishing simulation platform	getgophish.com
Zphisher	30+ phishing templates	git clone https://github.com/htr-tech/zphisher
NexPhisher	Multi-platform phishing tool	git clone https://github.com/htr-tech/nexphisher
Storm-Breaker	Access webcam/mic/location (SE)	git clone https://github.com/ultrasecurity/Storm-Breaker
Evilginx2	Man-in-the-middle reverse proxy	go install github.com/kgretzky/evilginx2@latest
Modlishka	Reverse proxy phishing framework	go install github.com/drk1wi/Modlishka@latest
King Phisher	Phishing campaign toolkit	github.com/rsmusllp/king-phisher
SocialFish	Social media phishing	git clone https://github.com/UndeadSec/SocialFish
AdvPhishing	Advanced phishing tool	git clone https://github.com/Ignitetch/AdvPhishing
URLCADIZ	URL masking tool	git clone https://github.com/PerezMascato/URLCADIZ
💻 Zphisher — Install & Usage
16. Vulnerability Scanning & Exploitation
💣 Frameworks for finding and verifying vulnerabilities on authorized targets.

⚠️ Always have written permission before running any of these tools.

Tool	Description	Install / Link
Metasploit	Industry-standard pen testing framework	apt install metasploit-framework
Nuclei	Template-based fast vulnerability scanner	go install github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest
SQLMap	Automated SQL injection tool	apt install sqlmap
Burp Suite	Web app security testing proxy	portswigger.net/burp
OWASP ZAP	Open-source web app scanner	zaproxy.org
OpenVAS	Open-source vulnerability scanner	apt install openvas
Commix	Command injection exploiter	git clone https://github.com/commixproject/commix
GoldenEye	HTTP DoS tool (authorized load testing)	git clone https://github.com/jseidl/GoldenEye
ExploitDB	Exploit database (searchsploit)	exploit-db.com
Criminal IP	Vulnerability & CVE search	criminalip.io
17. Network & Wireless Tools
📶 Analyze traffic, audit Wi-Fi networks, and perform MITM on authorized targets.

Tool	Description	Install / Link
Wireshark	Network protocol analyzer	apt install wireshark
Aircrack-ng	Wi-Fi security auditing suite	apt install aircrack-ng
Kismet	Wireless network detector & sniffer	apt install kismet
Bettercap	MITM framework (ARP, DNS, HTTP)	apt install bettercap
Ettercap	MITM attack suite	apt install ettercap-common
Wifite	Automated Wi-Fi auditing tool	apt install wifite
Reaver	WPS brute force tool	apt install reaver
Fern Wifi Cracker	GUI-based Wi-Fi audit tool	apt install fern-wifi-cracker
Fluxion	Wi-Fi social engineering (evil twin)	git clone https://github.com/FluxionNetwork/fluxion
hcxtools	Wi-Fi packet capture conversion	apt install hcxtools
Netcat	The TCP/IP swiss army knife	apt install netcat-openbsd
tcpdump	Command-line packet analyzer	apt install tcpdump
18. Mobile Hacking & Phone Exploitation
📲 Android/iOS security testing for authorized assessments.

Tool	Description	Install / Link
PhoneSploit	ADB-based phone exploitation	git clone https://github.com/aerosol-can/PhoneSploit
AhMyth Android RAT	Android remote access tool	git clone https://github.com/AhMyth/AhMyth-Android-RAT
Apktool	Android APK decompiler/rebuilder	apt install apktool
jadx	Android APK decompiler (GUI)	apt install jadx
Frida	Dynamic instrumentation toolkit	pip install frida-tools
Objection	Runtime mobile exploration	pip install objection
MobSF	Mobile Security Framework (static+dynamic)	github.com/MobSF/Mobile-Security-Framework-MobSF
MSFPC	MSF payload creator	git clone https://github.com/g0tmi1k/msfpc
19. AI-Powered OSINT & Free AI Tools
🤖 AI tools for automating research, analyzing images, and accelerating investigations.

Pro tip: Perplexity AI is excellent for OSINT research — it cites sources so you can verify everything.

AI-Powered OSINT Tools
Tool	Description	Install / Link
GeoSpy	AI geolocation from images	geospy.ai
DeepFace	Face analysis (age, gender, emotion)	pip install deepface
face_recognition	Python face recognition library	pip install face_recognition
OpenCV	Computer vision library	pip install opencv-python
ReconAIzer	AI-enhanced Burp Suite extension	github.com/hisxo/ReconAIzer
AI or Not	Detect AI-generated content	aiornot.com
HARPA AI	AI browser agent for OSINT	harpa.ai
Free AI Tools for OSINT Research
Tool	Description	Free Tier	Link
Claude	Best for reasoning & analysis	✅ Free tier	claude.ai
ChatGPT	OpenAI's AI assistant	✅ GPT-4o mini	chat.openai.com
Perplexity AI	AI search with cited sources	✅ 5 Pro/day	perplexity.ai
Google Gemini	Google AI with web search	✅ Free	gemini.google.com
DeepSeek	Open-source, strong reasoning	✅ Free	chat.deepseek.com
Grok	Real-time X/Twitter data	✅ Free on X	x.com/grok
Microsoft Copilot	AI with Bing search integration	✅ Free	copilot.microsoft.com
NotebookLM	Google's document analysis AI	✅ Free	notebooklm.google.com
Phind	AI search for developers	✅ Free	phind.com
HuggingChat	Open-source AI chat	✅ Free	huggingface.co/chat
20. Financial & Corporate Intelligence
💰 Research companies, track crypto, and uncover financial relationships.

Tool	Description	Link
OpenCorporates	Global corporate database	opencorporates.com
ICIJ Offshore Leaks	Panama/Pandora/Paradise Papers	offshoreleaks.icij.org
SEC EDGAR	US company filings	sec.gov/edgar
Companies House (UK)	UK company register	beta.companieshouse.gov.uk
Aleph (OCCRP)	Global corporate & public records	aleph.occrp.org
Orbit	Bitcoin address investigator	git clone https://github.com/s0md3v/Orbit
Blockchain.com	Bitcoin explorer	blockchain.com/explorer
Etherscan	Ethereum blockchain explorer	etherscan.io
BinCheck	Bank card BIN lookup	bincheck.io
Crunchbase	Company/startup database	crunchbase.com
LEI Search	Legal Entity Identifier lookup	search.gleif.org
21. Vehicle, Property & Public Records
🚗 Access public records, vehicle history, property data, and court documents.

Tool/Service	Description	Link
FAXVIN	Free VIN decoder	faxvin.com
AutoCheck	Vehicle history reports	autocheck.com
NICB VINCheck	Stolen vehicle check	nicb.org/vincheck
PACER	US federal court records	pacer.uscourts.gov
Zillow	Property records & estimates	zillow.com
Who Owns What	NYC landlord portfolio lookup	whoownswhat.justfix.org
FOIA.gov	Freedom of Information Act portal	foia.gov
Court Listener	Free US court opinion search	courtlistener.com
22. Metadata & Digital Forensics
🔬 Extract hidden data, recover deleted files, and analyze digital evidence.

Pro tip: CyberChef is a must-bookmark — it handles encoding, encryption, and data manipulation all in-browser.

Tool	Description	Install / Link
Autopsy	Full digital forensics platform	autopsy.com
Volatility	Memory forensics framework	pip install volatility3
Wireshark	Network packet analysis	apt install wireshark
Binwalk	Firmware analysis & extraction	apt install binwalk
Foremost	File carving (recover deleted files)	apt install foremost
Bulk Extractor	Extract features from disk images	apt install bulk-extractor
ExifTool	Complete metadata extraction	apt install libimage-exiftool-perl
Metagoofil	Document metadata harvester	pip install metagoofil
CyberChef	Data analysis swiss army knife	gchq.github.io/CyberChef
Scalpel	File carving tool	apt install scalpel
23. IP Camera & Webcam OSINT
⚠️ WARNING: Accessing cameras without authorization is illegal everywhere. This section is for educational awareness only — to understand how exposed devices are found so you can protect them.

Shodan Searches for Exposed Cameras
Search Query	What It Finds
screenshot.label:webcam	Webcams indexed by Shodan
port:554 has_screenshot:true	RTSP cameras with screenshots
Server: yawcam	Yawcam webcams
webcamXP	WebcamXP servers
port:8080 title:"Blue Iris"	Blue Iris CCTV
port:37777 "DVR"	Dahua DVR systems
port:80 title:"DVR"	Web-accessible DVR
Google Dorks for Camera Discovery
Google Dork	Target
inurl:"viewerframe?mode="	Axis network cameras
intitle:"webcamXP 5"	WebcamXP 5 servers
inurl:"videostream.cgi"	CGI video streams
intitle:"Live View / - AXIS"	AXIS cameras
inurl:/view/view.shtml	Mobotix cameras
24. Google Dorking Bible
🔍 Advanced search operators for finding information that isn't easily discoverable.

Pro tip: Combine multiple operators for maximum precision. Always test in a private/incognito window.

Core Operators
Operator	Description	Example
site:	Search within a domain	site:example.com admin
inurl:	Search in URL path	inurl:admin login
intitle:	Search in page title	intitle:"index of" passwords
intext:	Search in page body	intext:"username" "password"
filetype:	Search by file type	filetype:pdf "confidential"
ext:	Search by extension	ext:sql "dump"
cache:	View Google's cached version	cache:example.com
allintext:	All terms in page body	allintext:username password email
High-Value OSINT Dorks
Purpose	Google Dork
Exposed passwords	intitle:"index of" "passwords.txt"
SQL database dumps	filetype:sql "CREATE TABLE" "INSERT INTO"
Config files	ext:conf OR ext:cnf "password"
Exposed .env files	intitle:"index of" ".env"
Open FTP servers	intitle:"index of" inurl:ftp
Exposed git repos	intitle:"index of" ".git"
SSH private keys	filetype:pem "PRIVATE KEY"
phpinfo pages	ext:php intitle:phpinfo
Exposed log files	filetype:log "password" OR "username"
Dork Generator Tools
Tool	Link
DorkSearch	dorksearch.com
Google Hacking DB (GHDB)	exploit-db.com/google-hacking-database
Pagodo	git clone https://github.com/opsdisk/pagodo
GooFuzz	git clone https://github.com/m3n0sd0n4ld/GooFuzz
25. Credential & Data Dorking
🗄️ Advanced dorks for finding inadvertently exposed sensitive data on the web.

Purpose	Google Dork
Gmail in spreadsheets	allintext:"@gmail.com" "password" filetype:xlsx
Exposed credentials in CSV	filetype:csv "email" "password"
Pastebin credential dumps	filetype:txt "username" "password" site:pastebin.com
Database dumps	filetype:sql "INSERT INTO" "password" "email"
Config files with API keys	filetype:env "DB_PASSWORD" OR "API_KEY" OR "SECRET"
Exposed .htpasswd	filetype:htpasswd htpasswd
phpMyAdmin without auth	inurl:phpmyadmin/index.php intitle:"phpMyAdmin"
Exposed Jenkins	intitle:"Dashboard [Jenkins]" inurl:"/login"
AWS keys exposed	filetype:pem "AKIA" OR "ASIA"
GitHub secrets	site:github.com "API_KEY" OR "api_secret" filetype:env
26. IP Tracking & Geolocation Links
📍 Tools for tracking IP addresses through crafted links.

⚠️ For authorized use only — e.g., tracking your own email campaigns or authorized phishing simulations.

Tool	Description	Link
Grabify	IP grabber & URL shortener	grabify.link
IPLogger	IP logging URL shortener	iplogger.org
Canary Tokens	Tracking tokens (URL, email, DNS, files)	canarytokens.org
GetNotify	Email open tracking + geolocation	getnotify.com
IPinfo	IP address data API	ipinfo.io
IP-API	IP geolocation API	ip-api.com
MaxMind GeoIP	IP geolocation database	maxmind.com
💡 Trick: Mask a logger URL using the VK redirect: https://vk.com/away.php?to=YOUR_LOGGER_URL

27. Telegram OSINT Bots & Channels
💬 Telegram-based OSINT tools, bots, and intelligence communities.

OSINT Bots
Bot	Description	Handle
Eye of God (Glaz Boga)	Person lookup by phone/email/photo/VK	@glazzz_rus_bot
@No_BlackMail_bot	Search email by phone number	@No_BlackMail_bot
@OverSerchBot	Multi-search OSINT bot	@OverSerchBot
GetContact Bot	Phone number caller ID	@getcontact_real_bot
Quick OSINT	Fast person lookup	@Quick_OSINT_bot
@CreationDateBot	Check Telegram account creation date	@creationdatebot
@SangMataBot	Check username history of TG accounts	@SangMataInfo_bot
OSINT Channels
Channel	Content	Link
@overbafer1	Hacking & cybersecurity	t.me/overbafer1
@Social_engineering	Social engineering techniques	t.me/Social_engineering
@cyberbezopasno	Cybersecurity news & tools	t.me/cyberbezopasno
@OSINT_group	OSINT community	t.me/OSINT_group
Telegram Scraping Tools
Tool	Description	Install
Telepathy	Telegram OSINT analysis	pip install telepathy
Telethon	Python Telegram API library	pip install telethon
TeleGram-OSINTer	Telegram profile investigation	git clone https://github.com/Alb-310/TeleGram-OSINTer
28. Russian OSINT & Person Lookup Services
🇷🇺 Services widely used in Russian-speaking OSINT communities.

#	Service	Description	Link
1	FNS (Tax Service)	Get INN number, check tax debts	service.nalog.ru
2	TelPoisk	Phone directory — address by name	telpoisk.com
3	GetContact	See how number is saved by others	getcontact.com
4	Eye of God	Person lookup by phone/email/photo	@glazzz_rus_bot
5	Search4faces	Face search in VK & OK	search4faces.com
6	GetNotify	Email tracking + geolocation	getnotify.com
7	BinCheck	Card BIN lookup (bank, region)	bincheck.io
VK (VKontakte) OSINT
Purpose	Tool/URL
Registration data	regvk.com
FOAF data	https://vk.com/foaf.php?id=USER_ID
VK page archive	vk.watch/ID/profile
Activity tracking	nebaz.ru
VK tools	220vk.com
29. Social Media Searcher Platforms
Tool	Description	Free?	Link
Social Searcher	Real-time social media search	✅ Yes	social-searcher.com
Social Mention	Social media aggregator	✅ Yes	socialmention.com
Google Alerts	Free web monitoring	✅ Free	google.com/alerts
Who Posted What	Facebook keyword search	✅ Free	whopostedwhat.com
Mention	Social media & web monitoring	🟡 Freemium	mention.com
Talkwalker	Social listening & analytics	💰 Paid	talkwalker.com
BrandWatch	Social intelligence platform	💰 Paid	brandwatch.com
Hootsuite	Social media management	🟡 Freemium	hootsuite.com
30. Termux Hacking Toolkit (Complete)
📱 Full OSINT & security toolkit setup for Android via Termux.

Initial Setup
# First-time Termux setup
pkg update -y && pkg upgrade -y
pkg install python python2 git wget curl nmap
pip install requests colorama
termux-setup-storage
Tool List
#	Tool	Purpose	Install
1	Sherlock	Username OSINT	pip install sherlock-project
2	Maigret	Username OSINT (3000+ sites)	pip install maigret
3	h8mail	Email breach hunting	pip install h8mail
4	Zphisher	Phishing (30+ templates)	git clone https://github.com/htr-tech/zphisher
5	NexPhisher	Advanced phishing	git clone https://github.com/htr-tech/nexphisher
6	Storm-Breaker	Camera/Mic/Location SE	git clone https://github.com/ultrasecurity/Storm-Breaker
7	UserRecon	Username search	git clone https://github.com/wishihab/userrecon
8	IPGeoLocation	IP geolocation	git clone https://github.com/maldevel/IPGeoLocation
9	Orbit	Bitcoin address search	git clone https://github.com/s0md3v/Orbit
10	Nmap	Network scanner	pkg install nmap
11	Hydra	Login brute force	pkg install hydra
12	PhoneSploit	Phone exploitation via ADB	git clone https://github.com/aerosol-can/PhoneSploit
13	fsociety	All-in-one hacking pack	git clone https://github.com/Manisso/fsociety
💻 One-command Termux installer
31. Kali Linux OSINT Toolkit
🐉 Tools pre-installed on Kali, plus recommended additions.

Pre-installed on Kali
Tool	Category	Command
Nmap	Network scanning	nmap
Wireshark	Packet analysis	wireshark
Metasploit	Exploitation	msfconsole
SQLMap	SQL injection	sqlmap
Hydra	Brute force	hydra
John the Ripper	Password cracking	john
Hashcat	GPU password cracking	hashcat
Aircrack-ng	Wi-Fi cracking	aircrack-ng
Nikto	Web scanner	nikto
Dirb	Directory brute force	dirb
WPScan	WordPress scanner	wpscan
theHarvester	Email/subdomain OSINT	theHarvester
Maltego	Visual link analysis	maltego
Recon-ng	Web recon framework	recon-ng
SET	Social engineering toolkit	setoolkit
Burp Suite	Web proxy	burpsuite
Quick Kali Setup (additional tools)
# From this repo's installer (recommended — installs everything)
sudo bash install.sh

# Or add specific tools manually:
sudo apt update && sudo apt install -y \
  amass subfinder httpx nuclei gobuster feroxbuster \
  spiderfoot eyewitness phoneinfoga metagoofil

pip install maigret holehe h8mail socialscan social-analyzer \
  deepface face_recognition volatility3 telepathy
32. All-in-One Hacking Frameworks
🧰 Comprehensive frameworks that bundle dozens of tools under one roof.

Framework	Description	Install
fsociety	Mr. Robot-inspired hacking pack	git clone https://github.com/Manisso/fsociety
Hackingtool	All-in-one tool (100+ categories)	git clone https://github.com/Z4nzu/hackingtool
SpiderFoot	OSINT automation platform	pip install spiderfoot
Maltego	Visual OSINT & link analysis	Pre-installed in Kali
Recon-ng	Module-based recon framework	pip install recon-ng
Lazy Script	Automated pentest helper	git clone https://github.com/arismelachroinos/lscript
osmedeus	Full automated recon workflow	git clone https://github.com/j3ssie/osmedeus
33. Wordlist Generation & Brute Force
📖 Build custom wordlists or use proven collections.

Pro tip: CeWL is great for targeted attacks — it generates wordlists from the target's own website.

Tool	Description	Install
Crunch	Pattern-based wordlist generator	apt install crunch
CeWL	Custom wordlist from any website	apt install cewl
Cupp	Profile-based wordlist generator	git clone https://github.com/Mebus/cupp
SecLists	The ultimate security wordlist collection	git clone https://github.com/danielmiessler/SecLists
RockYou	Classic leaked password list	Pre-installed in Kali (/usr/share/wordlists/)
Weakpass	Massive wordlist collection	weakpass.com
💻 Wordlist Quick Reference
34. Hardware Hacking Tools
🔧 Physical devices for authorized penetration testing and hardware security research.

Device	Description	Price
Flipper Zero	Multi-tool: RFID, NFC, IR, Sub-GHz, BadUSB	~$170
HackRF One	Software-defined radio (1MHz–6GHz)	~$300
Proxmark3	RFID/NFC research & cloning tool	~$60–300
WiFi Pineapple	Wi-Fi auditing & rogue AP platform	~$100–300
USB Rubber Ducky	USB keystroke injection device	~$80
Bash Bunny	Multi-function USB attack platform	~$120
LAN Turtle	Covert network access & MITM	~$60
RTL-SDR	Budget software-defined radio dongle	~$25
Alfa AWUS036ACH	Long-range dual-band Wi-Fi adapter	~$50
O.MG Cable	USB cable with embedded implant	~$120
35. OSINT Operating Systems
🖥️ Specialized operating systems built for security research, OSINT, and privacy.

OS	Focus	Link
Kali Linux	Penetration testing (600+ tools)	kali.org
Parrot OS	Security & privacy	parrotsec.org
Tails	Privacy & anonymity (amnesic)	tails.boum.org
Whonix	Anonymous OS via Tor	whonix.org
CSI Linux	OSINT & forensics focused	csilinux.com
Trace Labs OSINT VM	OSINT-specific VM	tracelabs.org
BlackArch	2800+ security tools	blackarch.org
SIFT Workstation	SANS digital forensics	digital-forensics.sans.org
REMnux	Malware analysis	remnux.org
Qubes OS	Security via compartmentalization	qubes-os.org
CommandoVM	Windows pentest VM	github.com/mandiant/commando-vm
36. OSINT APIs & Developer Tools
🔌 Programmatic access to OSINT data sources for building your own tools.

API	Description	Link
Shodan API	IoT/device search	developer.shodan.io
VirusTotal API	File/URL analysis	developers.virustotal.com
Hunter.io API	Email discovery	hunter.io/api
Have I Been Pwned API	Breach check	haveibeenpwned.com/API
IPinfo API	IP geolocation	ipinfo.io/developers
Censys API	Internet scanning	search.censys.io/api
GitHub API	Repository/user data	api.github.com
Dehashed API	Breach data search	dehashed.com/docs
urlscan.io API	URL analysis	urlscan.io/docs/api
AbuseIPDB API	IP reputation	abuseipdb.com/api
Google Custom Search API	Programmable search	developers.google.com/custom-search
WhoisXML API	Domain intelligence	whoisxmlapi.com
Criminal IP API	Threat intelligence	criminalip.io/developer
37. Browser Extensions for OSINT
🧩 Must-have browser extensions for every OSINT investigator.

Extension	Description	Browser
Search by Image	Multi-engine reverse image search	Chrome / Firefox
Wappalyzer	Technology stack detector	Chrome / Firefox
Shodan	Server info on any website	Chrome / Firefox
Wayback Machine	View archived pages instantly	Chrome / Firefox
EXIF Viewer	View image metadata	Chrome / Firefox
User-Agent Switcher	Change browser identity	Chrome / Firefox
FoxyProxy	Proxy management	Chrome / Firefox
Hunchly	OSINT web capture & case manager	Chrome
InVID/WeVerify	Video/image verification	Chrome / Firefox
SingleFile	Save complete web pages	Chrome / Firefox
38. OSINT Learning Resources
📚 The best resources for learning OSINT — from beginner to professional.

Resource	Type	Link
OSINT Framework	Interactive tool directory	osintframework.com
IntelTechniques	Michael Bazzell's resources & podcast	inteltechniques.com
Bellingcat	OSINT investigative journalism	bellingcat.com
Trace Labs	OSINT for missing persons CTFs	tracelabs.org
OSINT Curious Project	Community & training	osintcurio.us
Sector035 Week in OSINT	Weekly OSINT newsletter	sector035.nl
OSINT Dojo	Training platform & challenges	osintdojo.com
CTF Time	Hands-on CTF competitions	ctftime.org
GIJN	Global Investigative Journalism Network	gijn.org
SANS OSINT	Professional cyber training	sans.org
📺 YouTube Channels
Channel	Focus
John Hammond	Cybersecurity & CTFs
The Cyber Mentor	Ethical hacking
David Bombal	Networking & security
NetworkChuck	Cybersecurity tutorials
HackerSploit	Penetration testing
Null Byte	Hacking tutorials
13Cubed	DFIR & forensics
39. Awesome OSINT GitHub Repos
⭐ The best curated OSINT resource lists on GitHub.

Repository	Stars	Link
jivoi/awesome-osint	20k+	github.com/jivoi/awesome-osint
danielmiessler/SecLists	55k+	github.com/danielmiessler/SecLists
Z4nzu/hackingtool	40k+	github.com/Z4nzu/hackingtool
cipher387/osint_stuff_tool_collection	6k+	github.com/cipher387/osint_stuff_tool_collection
Manisso/fsociety	10k+	github.com/Manisso/fsociety
sinwindie/OSINT	3k+	github.com/sinwindie/OSINT
Astrosp/Awesome-OSINT-For-Everything	2k+	github.com/Astrosp/Awesome-OSINT-For-Everything
tracelabs/awesome-osint	1k+	github.com/tracelabs/awesome-osint
40. One-Click Install Scripts
🐉 Kali Linux — Full Arsenal
# Option 1: Direct from this repo (one command)
curl -sL https://raw.githubusercontent.com/rawfilejson/awesome-osint-arsenal/main/install.sh | sudo bash

# Option 2: Clone first (recommended — inspect before running)
git clone https://github.com/rawfilejson/awesome-osint-arsenal.git
cd awesome-osint-arsenal
sudo bash install.sh
📱 Termux (Android)
pkg update -y && pkg upgrade -y
pkg install -y python git wget curl nmap hydra perl openssh php clang make openssl
pip install requests colorama sherlock-project maigret holehe h8mail
cd ~ && git clone https://github.com/htr-tech/zphisher && git clone https://github.com/Manisso/fsociety
🔧 Manual Kali Snippet
sudo apt update && sudo apt upgrade -y
sudo apt install -y git python3 python3-pip golang-go nmap wireshark \
  sqlmap hydra john hashcat aircrack-ng nikto dirb wpscan \
  theharvester maltego spiderfoot set exiftool masscan whatweb \
  gobuster feroxbuster wfuzz libimage-exiftool-perl binwalk \
  foremost bulk-extractor macchanger tor proxychains4

pip3 install sherlock-project maigret holehe h8mail socialscan \
  social-analyzer phoneinfoga snscrape instaloader deepface \
  face_recognition volatility3 blackbird-osint nexfil \
  socid-extractor osrframework telepathy twayback toutatis \
  dnstwist waybackpy trufflehog

cd /opt
sudo git clone https://github.com/Manisso/fsociety
sudo git clone https://github.com/Z4nzu/hackingtool
sudo git clone https://github.com/ultrasecurity/Storm-Breaker
sudo git clone https://github.com/htr-tech/zphisher
sudo git clone https://github.com/s0md3v/Orbit
sudo git clone https://github.com/s0md3v/Photon
sudo git clone https://github.com/danielmiessler/SecLists
sudo git clone https://github.com/lgandx/Responder
sudo git clone https://github.com/commixproject/commix
sudo git clone https://github.com/opsdisk/pagodo
sudo git clone https://github.com/RedSiege/EyeWitness
41. Top 50 Must-Have Tools (Quick Reference)
#	Tool	Category	Install
1	Sherlock	Username OSINT	pip install sherlock-project
2	Maigret	Username OSINT (3000+ sites)	pip install maigret
3	h8mail	Email breach hunting	pip install h8mail
4	Holehe	Email registration check	pip install holehe
5	theHarvester	Domain/email recon	apt install theharvester
6	PhoneInfoga	Phone number OSINT	See install guide
7	Nmap	Network scanning	apt install nmap
8	Amass	DNS enumeration	go install ...amass@master
9	Subfinder	Subdomain discovery	go install ...subfinder@latest
10	Nuclei	Vulnerability scanning	go install ...nuclei@latest
11	SQLMap	SQL injection	apt install sqlmap
12	Metasploit	Exploitation framework	apt install metasploit-framework
13	Hashcat	Password cracking (GPU)	apt install hashcat
14	Hydra	Login brute force	apt install hydra
15	Wireshark	Network analysis	apt install wireshark
16	Aircrack-ng	Wi-Fi security	apt install aircrack-ng
17	Burp Suite	Web proxy/testing	portswigger.net
18	SpiderFoot	OSINT automation	pip install spiderfoot
19	Maltego	Visual link analysis	Pre-installed in Kali
20	Recon-ng	Recon framework	pip install recon-ng
21	PimEyes	Face search engine	pimeyes.com
22	Shodan	IoT device search	shodan.io
23	Censys	Internet scanning	censys.io
24	Zphisher	Phishing tool	git clone .../zphisher
25	Storm-Breaker	Camera/mic SE tool	git clone .../Storm-Breaker
26	ExifTool	Image metadata	apt install libimage-exiftool-perl
27	Autopsy	Digital forensics	autopsy.com
28	Volatility	Memory forensics	pip install volatility3
29	Tor Browser	Anonymous browsing	torproject.org
30	DeHashed	Breach search engine	dehashed.com
31	Have I Been Pwned	Breach checker	haveibeenpwned.com
32	fsociety	All-in-one framework	git clone .../fsociety
33	Hackingtool	100+ tools in one	git clone .../hackingtool
34	SecLists	Security wordlists	git clone .../SecLists
35	Osintgram	Instagram OSINT	git clone .../Osintgram
36	VirusTotal	Malware/file analysis	virustotal.com
37	Canary Tokens	IP tracking tokens	canarytokens.org
38	CyberChef	Data analysis tool	gchq.github.io/CyberChef
39	DeepFace	AI face analysis	pip install deepface
40	dnsrecon	DNS enumeration	pip install dnsrecon
41	Gobuster	Directory brute-force	go install ...gobuster@latest
42	HTTPx	HTTP probing	go install ...httpx@latest
43	EyeWitness	Web screenshots	git clone .../EyeWitness
44	Responder	LLMNR/NBT-NS poisoner	git clone .../Responder
45	Bettercap	MITM framework	apt install bettercap
46	Photon	Web OSINT crawler	git clone .../Photon
47	Perplexity AI	AI research assistant	perplexity.ai
48	GeoSpy	AI image geolocation	geospy.ai
49	osmedeus	Full recon workflow	git clone .../osmedeus
50	trufflehog	Git secret scanner	pip install trufflehog
☕ Liked everything above? Section 42-50 just dropped — fuel the next batch:

Buy Me a Coffee

42. ⚔️ Red Team & Offensive Security
C2 frameworks, AD attacks, exploitation kits, post-exploitation. Authorized testing only.

Pro tip: Sliver and Havoc are the modern open-source Cobalt Strike alternatives — start there before paying.

Tool	Description	Install / Link
AD Attack & Defense	Comprehensive Active Directory attack reference	git clone https://github.com/infosecn1nja/AD-Attack-Defense.git
Arjun	HTTP parameter discovery suite	pip3 install arjun
BloodHound	AD attack-path graph analysis	git clone https://github.com/BloodHoundAD/BloodHound.git
BloodHound CE	Community Edition of BloodHound — modernized stack	docker pull specterops/bloodhound:latest
Brute Ratel C4	Premium C2 with strong AV/EDR evasion	bruteratel.com
Certipy	Active Directory Certificate Services enumeration and abuse	pip3 install certipy-ad
Cobalt Strike	Premium adversary simulation / red team framework	cobaltstrike.com
CrackMapExec	Post-exploitation tool for AD networks	pip3 install crackmapexec
CRLFuzz	Fast CRLF-injection scanner in Go	go install github.com/dwisiswant0/crlfuzz/cmd/crlfuzz@latest
Dalfox	Fast, intelligent XSS scanner	go install github.com/hahwul/dalfox/v2@latest
Evil-WinRM	Ultimate WinRM shell for hacking/pentesting	apt install evil-winrm
Ghauri	Advanced cross-platform tool to detect/exploit SQLi	git clone https://github.com/r0oth3x49/ghauri.git
Gxss	Test parameters for cross-site scripting reflection	go install github.com/KathanP19/Gxss@latest
HackTricks	Pentesting / hacking knowledge base by carlospolop	book.hacktricks.xyz
Havoc	Modern, malleable post-exploitation C2 framework	git clone https://github.com/HavocFramework/Havoc.git
Impacket	Python classes for working with network protocols (Windows attacks)	pip3 install impacket
Kerbrute	Tool for performing Kerberos pre-auth bruteforcing	go install github.com/ropnop/kerbrute@latest
kiterunner	Contextual content-discovery for modern API endpoints	go install github.com/assetnote/kiterunner/cmd/kr@latest
Merlin	Cross-platform HTTP/2 post-exploitation server and agent in Go	go install github.com/Ne0nd0g/merlin@latest
Metasploit Framework	Industry-standard exploitation framework with 2000+ modules	apt install metasploit-framework
Mythic	Cross-platform, post-exploit, multi-user red team framework	git clone https://github.com/its-a-feature/Mythic.git
NetExec (nxc)	CrackMapExec maintained successor — AD network exploitation	pip3 install git+https://github.com/Pennyw0rth/NetExec
Nighthawk	Premium evasive C2 by MDSec (Cobalt Strike alt)	mdsec.co.uk
NoSQLMap	Automated NoSQL database enumeration and exploitation	git clone https://github.com/codingo/NoSQLMap.git
Nuclei Templates	Community-curated templates for Nuclei	git clone https://github.com/projectdiscovery/nuclei-templates.git
ParamMiner (Burp ext)	Discover hidden, unlinked HTTP parameters in Burp	git clone https://github.com/PortSwigger/param-miner.git
PayloadsAllTheThings	Web app pentest payloads, bypasses, and methodology	git clone https://github.com/swisskyrepo/PayloadsAllTheThings.git
PetitPotam	PoC tool to coerce Windows hosts to authenticate to attacker	git clone https://github.com/topotam/PetitPotam.git
PowerShell Empire	Post-exploitation framework with PS-based agents	git clone https://github.com/BC-SECURITY/Empire.git
Rubeus	C# toolset for raw Kerberos interaction and abuse	git clone https://github.com/GhostPack/Rubeus.git
SharpHound	C# data collector for BloodHound	git clone https://github.com/BloodHoundAD/SharpHound.git
Sliver	Open-source adversary emulation/red-team framework (Cobalt Strike alt)	go install github.com/bishopfox/sliver/server@latest
SSRFmap	Automated SSRF detection and exploitation framework	git clone https://github.com/swisskyrepo/SSRFmap.git
Villain	High-level stage 0/1 C2 framework for handling sibling agents	git clone https://github.com/t3l3machus/Villain.git
XSStrike	Advanced XSS scanner with crawler and payload generator	git clone https://github.com/s0md3v/XSStrike.git
43. 🛡️ Blue Team & Defensive Security
SIEM, EDR, network monitoring, detection engineering, IR.

Pro tip: Wazuh is your free Splunk replacement. Pair it with Sigma rules + Suricata for a full SOC stack on commodity hardware.

Tool	Description	Install / Link
Atomic Red Team	Library of small detection-test scripts mapped to MITRE ATT&CK	git clone https://github.com/redcanaryco/atomic-red-team.git
Chainsaw	Hunt threats in Windows event logs — fast forensics	git clone https://github.com/WithSecureLabs/chainsaw.git
Cortex (TheHive)	Observable analysis and active response engine	docker pull thehiveproject/cortex:latest
Elastic Stack (ELK)	Elasticsearch + Logstash + Kibana — log analytics	docker pull docker.elastic.co/elasticsearch/elasticsearch:latest
Falco	Cloud-native runtime security	git clone https://github.com/falcosecurity/falco.git
Graylog	Open-source log management / SIEM	docker pull graylog/graylog:latest
Hayabusa	Windows event log fast forensics timeline generator	git clone https://github.com/Yamato-Security/hayabusa.git
Loki	Simple IOC and YARA scanner by Florian Roth	git clone https://github.com/Neo23x0/Loki.git
MITRE ATT&CK	Adversary tactics, techniques, and procedures knowledge base	attack.mitre.org
MITRE CALDERA	Cyber adversary emulation platform	git clone https://github.com/mitre/caldera.git
MITRE D3FEND	Defensive countermeasure knowledge graph	d3fend.mitre.org
osquery	SQL-powered OS instrumentation/monitoring/analytics	apt install osquery
RITA	Real Intelligence Threat Analytics — beaconing/long-conn detection	git clone https://github.com/activecm/rita.git
Security Onion	Linux distro for threat hunting, monitoring, and log management	securityonionsolutions.com
Sigma	Generic signature format for SIEM detections	git clone https://github.com/SigmaHQ/sigma.git
sigma-cli	Convert Sigma rules to native SIEM queries	pip3 install sigma-cli
Snort	Open-source intrusion-prevention/detection system	apt install snort
Suricata	High-perf network IDS / IPS / NSM	apt install suricata
TheHive	Scalable, free, open-source case management for SOCs	docker pull strangebee/thehive:latest
Tracee	Runtime security and forensics using eBPF (Aqua)	git clone https://github.com/aquasecurity/tracee.git
Velociraptor	Endpoint visibility and digital forensics — query-driven	git clone https://github.com/Velocidex/velociraptor.git
Velociraptor Server	Centralized server for Velociraptor agents	docs.velociraptor.app
Wazuh	Open-source XDR / SIEM platform	git clone https://github.com/wazuh/wazuh.git
Zeek (Bro)	Powerful network analysis framework for security monitoring	apt install zeek
44. 🛰️ Threat Intel Platforms
CTI platforms — open-source and enterprise.

Pro tip: MISP is free and powerful. OpenCTI gives you a STIX2-native graph DB. Both run as Docker stacks.

Tool	Description	Install / Link
Anomali ThreatStream	Enterprise threat intel aggregation platform	anomali.com
CrowdStrike Falcon Intelligence	Premium adversary intel from CrowdStrike	crowdstrike.com
Digital Shadows SearchLight	Brand protection + dark web monitoring (now ReliaQuest GreyMatter DRP)	reliaquest.com
EclecticIQ Intelligence Center	STIX/TAXII-native threat intel platform	eclecticiq.com
Flashpoint	Business risk intel from criminal forums and dark web	flashpoint.io
Intel471	Premium adversary intelligence and underground monitoring platform	intel471.com
IntSights	External threat protection and intel (now part of Rapid7)	intsights.com
KELA	Cybercrime intelligence and dark-web monitoring	kelacyber.com
Mandiant Advantage	Threat intel from Google's Mandiant team	mandiant.com
OpenCTI	Open-source CTI platform structured around STIX2	docker pull opencti/platform
SOCRadar	Extended threat intel — attack surface + dark web + brand	socradar.io
ThreatConnect	Threat intel platform combining intel and SOAR	threatconnect.com
ThreatQ	Threat intel platform for SOCs	threatq.com
Yeti	Open distributed threat intelligence platform	git clone https://github.com/yeti-platform/yeti.git
45. 🔬 Digital Forensics & Reverse Engineering
Disk/memory forensics, malware reverse engineering, timeline tools, binary analysis.

Pro tip: Volatility 3 + Plaso (log2timeline) + KAPE = the modern DFIR triage stack. Ghidra > IDA Free for static analysis.

Tool	Description	Install / Link
Binary Ninja	Modern reverse engineering platform with API	binary.ninja
Cutter	GUI for radare2/rizin reverse-engineering	git clone https://github.com/rizinorg/cutter.git
Dissect	Fox-IT framework for fast forensic image analysis	pip3 install dissect
Eric Zimmerman's Tools	Suite of free Windows DFIR utilities	ericzimmerman.github.io
FTK Imager	Forensic disk imaging tool by AccessData	exterro.com
Ghidra	NSA's open-source software reverse engineering suite	git clone https://github.com/NationalSecurityAgency/ghidra.git
IDA Free	Free version of IDA disassembler/decompiler	hex-rays.com
KAPE	Kroll Artifact Parser and Extractor — fast triage collection	kroll.com
PhotoRec	File data recovery — focuses on multimedia	apt install testdisk
Plaso (log2timeline)	Super-timeline creation from forensic artifacts	pip3 install plaso
radare2	Reverse engineering framework	apt install radare2
RegRipper	Open-source Windows registry parsing tool	git clone https://github.com/keydet89/RegRipper3.0.git
Rekall	Memory forensics tooling (legacy fork of Volatility)	pip3 install rekall
rizin	Modern fork of radare2 with cleaner API	git clone https://github.com/rizinorg/rizin.git
The Sleuth Kit	Library and CLI tools for forensic disk analysis	apt install sleuthkit
Volatility 3	Memory forensics framework	pip3 install volatility3
46. 🎓 Training, Labs & CTF
Hands-on practice — paid platforms and free local labs.

Pro tip: Free path: TryHackMe → PortSwigger Academy → HackTheBox retired boxes. Paid path: HTB Academy + OffSec PG.

Tool	Description	Install / Link
BugBountyHunter	Web hacking training and labs	bugbountyhunter.com
CTFtime	Calendar of upcoming and past CTF events	ctftime.org
Cybrary	Free + paid cybersecurity courses	cybrary.it
DVWA	Damn Vulnerable Web Application — classic appsec lab	git clone https://github.com/digininja/DVWA.git
Hack The Box	Online pentesting labs and CTFs	hackthebox.com
Hacker101	Free HackerOne course library and CTF	hacker101.com
Immersive Labs	Cyber skills platform with hands-on exercises	immersivelabs.com
Metasploitable	Intentionally vulnerable Linux VM for Metasploit practice	docs.rapid7.com
OffSec Proving Grounds	OSCP-style training labs by Offensive Security	offsec.com
OverTheWire Wargames	Free wargames for learning offensive security from scratch	overthewire.org
OWASP Juice Shop	Modern, intentionally insecure web app — covers OWASP Top 10	docker pull bkimminich/juice-shop
OWASP WebGoat	Deliberately insecure Java-based web app for training	docker pull webgoat/webgoat
PentesterLab	Hands-on web-app pentesting training	pentesterlab.com
picoCTF	Free CTF and learning platform built by CMU	picoctf.org
PortSwigger Web Security Academy	Free, world-class web security training (by Burp Suite team)	portswigger.net
pwn.college	Free college-level cybersecurity education from ASU	pwn.college
PwnedHub	Intentionally-vulnerable web app for hands-on appsec training	git clone https://github.com/practisec/pwnedhub.git
Root-Me	500+ challenges and 100+ virtual labs	root-me.org
TryHackMe	Beginner-friendly cybersecurity training platform	tryhackme.com
VulnHub	Free downloadable vulnerable VMs for offline practice	vulnhub.com
VulnYX	Online platform with vulnerable boxes (free + premium)	vulnyx.com
47. 🎯 Bug Bounty Platforms
Where to actually earn money from your skills.

Pro tip: Start on Bugcrowd or YesWeHack public programs — easier triage and lower competition than HackerOne H1.

Tool	Description	Install / Link
Bugbase	Indian-origin bug-bounty + vulnerability disclosure platform	bugbase.ai
Bugcrowd	Crowdsourced security platform — bug bounty + pentesting	bugcrowd.com
Disclose.io	Standardized vulnerability-disclosure language and tools	disclose.io
HackerOne	Largest bug-bounty platform — public and private programs	hackerone.com
HackTrophy	European bug-bounty platform	hacktrophy.com
Immunefi	Web3 / crypto-focused bug bounty platform	immunefi.com
Intigriti	European bug-bounty platform with fast triage	intigriti.com
Open Bug Bounty	Free coordinated-disclosure platform	openbugbounty.org
Public Bug Bounty Programs (chaos)	ProjectDiscovery's free BBH program list	chaos.projectdiscovery.io
Synack	Crowdsourced + vetted-researcher pentesting platform	synack.com
YesWeHack	European-based bug-bounty and VDP platform	yeswehack.com
Zerodium	Premium 0day acquisition platform	zerodium.com
48. 📚 Learning Resources
Books, courses, blogs, YouTube channels, awesome lists.

Pro tip: IppSec.rocks indexes EVERY HackTheBox walkthrough — search any retired box and watch how a pro solves it.

Tool	Description	Install / Link
0xdf hacks stuff	HTB writeups and pentesting writeups	0xdf.gitlab.io
awesome-hacking-resources	Beginner-friendly hacking learning resources	github.com
awesome-incident-response	Curated list of IR tools and resources	github.com
awesome-malware-analysis	Curated list of malware-analysis tools	github.com
awesome-pentest	Massive curated list of pentesting tools and resources	github.com
Bellingcat's Online Investigations Toolkit	Bellingcat-curated tools and methodology guide	bellingcat.com
BTFM: Blue Team Field Manual	Concise blue-team incident response reference	amazon.com
Hacking: The Art of Exploitation (book)	Classic by Jon Erickson — low-level attack fundamentals	nostarch.com
IppSec.rocks	Indexed walkthroughs of HackTheBox machines (video)	ippsec.rocks
John Hammond	Cybersecurity YouTube — CTFs, malware, walkthroughs	youtube.com
Linux for OSINT (cipher387)	21-day Linux-for-OSINT course (free)	git clone https://github.com/cipher387/linux-for-OSINT-21-days.git
LiveOverflow	Hacking and security YouTube — deep technical content	youtube.com
NahamSec	Bug bounty and offensive security YouTube content	youtube.com
Netlas Cookbook	Free OSINT automation cookbook	academy.netlas.io
OSINT Curious	Community blog, podcast, and learning resources	osintcurio.us
OSINT Techniques	Michael Bazzell's resources, books, and search tools	inteltechniques.com
Python for OSINT (cipher387)	21-day Python-for-OSINT course (free)	git clone https://github.com/cipher387/python-for-OSINT-21-days.git
Real-World Bug Hunting (book)	Peter Yaworski — bug bounty methodology and real reports	nostarch.com
RTFM: Red Team Field Manual	Concise red-team command reference	amazon.com
The Web Application Hacker's Handbook (book)	Stuttard & Pinto — appsec bible	amazon.com
49. ✨ Extra Tools (curated additions)
Tools added in v2.x — modern recon, archive lookups, niche services, research-grade pivots.

Pro tip: This section gets refreshed every release — check before you reach for an older tool.

Tool	Description	Install / Link
abuse.ch Hunting	Hunt across all abuse.ch malware platforms with one query	hunting.abuse.ch
Aleph Open Search	Dark-web search engine by Aleph Networks	open-search.aleph-networks.eu
Aletheia (image forensics)	Detect manipulated/AI-generated images	aletheia.ai
altdns	Generates permutations, alterations and mutations of subdomains	pip3 install py-altdns
anew	Append lines from stdin to a file only if not already there	go install github.com/tomnomnom/anew@latest
ANY.RUN	Interactive online malware sandbox	any.run
Apollo.io	B2B phone/email finder — 1200 free credits/yr	apollo.io
APT Groups and Operations	Spreadsheet of threat actors, sponsoring countries, TTPs	docs.google.com
Aquatone	Visual inspection of websites across hosts (HTTP screenshots, attack-surface flyovers)	go install github.com/michenriksen/aquatone@latest
Archive.today	Web archive — saves snapshots even when robots.txt blocks Wayback	archive.ph
Arctic Shift	Tool for accessing large dumps of Reddit data via API/web	git clone https://github.com/ArthurHeitmann/arctic_shift.git
Arkham Intelligence	On-chain intel — labels, entities, historical flows	arkhamintelligence.com
assetfinder	Find domains and subdomains related to a given domain	go install github.com/tomnomnom/assetfinder@latest
AutoRecon	Multi-threaded network reconnaissance and enumeration framework	pip3 install git+https://github.com/Tib3rius/AutoRecon.git
Axiom	Dynamic infra framework for parallel cloud-based recon	git clone https://github.com/pry0cc/axiom.git
BackgroundChecks.com	Background check aggregator (BeenVerified family)	backgroundchecks.com
Baidu	Major Chinese search engine — essential for China-focused OSINT	baidu.com
BeVigil	Search subdomains, URLs, parameters from mobile applications	bevigil.com
BGP.tools	Modern BGP toolkit for network reconnaissance	bgp.tools
BinaryEdge	Cyber risk and attack-surface intelligence	binaryedge.io
Bitquery	Blockchain data APIs for on-chain investigation	bitquery.io
Black Book Online	Free nationwide directory of public-record lookups	blackbookonline.info
BlackEye	32+ phishing template builder for credential capture (lab-only)	git clone https://github.com/An0nUD4Y/blackeye.git
Brave Browser	Privacy-focused browser with built-in Tor/IPFS support	brave.com
Brave Search	Independent, transparent, ad-free search engine	search.brave.com
BreachForums Status	Status tracking for the rotating BreachForums mirrors	breachforums.cx
Breadcrumbs	Free crypto investigation platform — visualize transaction flows	breadcrumbs.app
BrightCloud Threat Intelligence	URL/IP/threat reputation database	brightcloud.com
BrightCloud URL/IP Lookup	Reputation, category, and threat checks for URLs/IPs	brightcloud.com
BscScan	Binance Smart Chain explorer — same UX as Etherscan	bscscan.com
CachedView	View Google/Bing/Yandex cached versions of any page	cachedview.com
Castrick	Find social media accounts via email, username, phone	castrickclues.com
Censys CLI	Official Python wrapper and CLI for Censys	pip3 install censys
CertKit Certificate Search	Fast search for public SSL/TLS certificate records	certkit.io
Chainabuse	Public crypto-scam reporting database	chainabuse.com
Chainalysis Reactor	Premium blockchain investigation platform	chainalysis.com
CheckUser	Search username across multiple social networks	checkuser.vercel.app
CIRCL Hashlookup	Free public hashlookup for known software files	circl.lu
Cisco Talos Intelligence	IP and Domain Reputation Center for real-time detection	talosintelligence.com
Clearbit Connect	Email finder browser extension with company data	connect.clearbit.com
Cloudflare Radar	Internet traffic patterns, attacks, technology trends	radar.cloudflare.com
Clustrmaps	Find people and address information	clustrmaps.com
Commander Search	Boolean search builder for OSINT investigators	commandersearch.com
Constella Intelligence	Identity threat intel from breaches and dark web	constellaintelligence.com
ContactOut	Find emails and phones for 300M+ professionals	contactout.com
CredenShow	Identify your compromised credentials before others do	credenshow.com
CrossLinked	LinkedIn enumeration — generate username lists from LinkedIn profiles	pip3 install crosslinked
DBpedia	Structured Wikipedia data — SPARQL endpoint	dbpedia.org
Digital Footprint Check	Free username check on hundreds of sites	digitalfootprintcheck.com
dirsearch	Web path scanner — advanced wordlist-based directory bruteforce	pip3 install dirsearch
Discord Lookup	Look up Discord user info via ID	discordlookup.com
DiscordHistory	Search public Discord servers and messages	disboard.org
DNS History	Historical DNS records lookup	dnshistory.org
DocumentCloud	Platform for analyzing, annotating, publishing documents	documentcloud.org
DomainEye Reverse WHOIS	Search domains by registrant data	domaineye.com
dork-cli	Run Google dorks from the command line	git clone https://github.com/jgor/dork-cli.git
DorkGenius	AI-powered search query generator for Google, Bing, DuckDuckGo	dorkgenius.com
Dorky	Online dork builder for Google/Bing/DuckDuckGo	dorky.io
Dune Analytics	SQL queries over indexed blockchain data	dune.com
Elliptic	Crypto financial-crime detection and investigation	elliptic.co
EmailRep.io	Free email reputation API by Sublime Security	emailrep.io
Epieos Tools	Reverse-lookup email/phone for Google profile data	tools.epieos.com
Epstein Exposed	Searchable database of 2M+ DOJ Epstein case docs and network graphs	epsteinexposed.com
ETDA APT Groups	Search threat-actor groups and their tools	apt.etda.or.th
etherscan-py	Python wrapper for Etherscan API	pip3 install etherscan-python
ExportData	Historical tweet, follower, and trend export tool	exportdata.io
FamilyTreeNow	Free genealogy search — addresses, phones, emails	familytreenow.com
ffuf	Fast Go-based web fuzzer — directory, parameter, vhost discovery	go install github.com/ffuf/ffuf/v2@latest
Filesec.io	Catalog of malicious file extensions, risks, OS-level mitigations	filesec.io
Findomain	Cross-platform subdomain enumerator with monitoring features	git clone https://github.com/Findomain/Findomain.git
Flickr	Photo-sharing — geosearch + license + camera EXIF intact	flickr.com
Foller.me	Twitter analytics — bio, languages, hashtags, mentions	foller.me
Forensically Beta	Online image forensics — clone detection, level sweep	29a.ch
FullContact	Identity-resolution API and person enrichment	fullcontact.com
gau (getallurls)	Fetch URLs from AlienVault OTX, Wayback, Common Crawl, URLScan	go install github.com/lc/gau/v2/cmd/gau@latest
Geocreepy	Geolocation aggregator — pulls geotagged posts across networks	geocreepy.com
GeoHints	Browser-based satellite/streetview geolocation training & investigation	geohints.com
GeoSpy Pro	Premium AI image geolocation by Graylark	geospy.ai
Get-Metadata.com	Online EXIF extractor — handles .DOCX/.PDF too	get-metadata.com
gf	Wrapper around grep with patterns for bug-bounty workflow	go install github.com/tomnomnom/gf@latest
Ghiro	Automated digital image forensics	getghiro.org
git-hound	Find sensitive data exposed via GitHub code search	go install github.com/tillson/git-hound@latest
github_monitor	Real-time tracking of GitHub user activity and repo changes	git clone https://github.com/misiektoja/github_monitor.git
gitleaks	Detect secrets, credentials, and API keys in git repos	go install github.com/gitleaks/gitleaks/v8@latest
Google Guide Advanced Operators	Reference for Google search operators	googleguide.com
Google Hacking Database (GHDB)	Index of dorks for finding publicly exposed info	exploit-db.com
GoSpider	Fast Go web spider for crawling/audit	go install github.com/jaeles-project/gospider@latest
gowitness	Modern Go-based web screenshot utility (Aquatone successor)	go install github.com/sensepost/gowitness@latest
GrayhatWarfare	Index of open Amazon S3 buckets — find exposed cloud data	grayhatwarfare.com
GreyNoise CLI	Command-line tool for GreyNoise mass-scanner intel	pip3 install greynoise
GreyNoise Visualizer	Tells you which IPs are noise vs targeted threats	viz.greynoise.io
hakrawler	Fast Go web crawler for endpoint and asset discovery	go install github.com/hakluke/hakrawler@latest
Hatching Triage	Modern malware sandbox with kernel-level monitoring	tria.ge
haveibeenzuckered	Check if a phone number is in the 533M Facebook breach	haveibeenzuckered.com
HIB Ransomed	Check if your data has been leaked by ransomware groups	haveibeenransom.com
httprobe	Take a list of domains and probe for working HTTP/HTTPS	go install github.com/tomnomnom/httprobe@latest
Hudson Rock	Free infostealer-compromise check tools (domain/email/IP)	hudsonrock.com
Hybrid Analysis	Free advanced malware analysis service by CrowdStrike	hybrid-analysis.com
IKnowYour.Dad	Data breach search engine	iknowyour.dad
Imgur	Image hosting — meme tracing and reverse search	imgur.com
instagram_monitor	Real-time tracking of Instagram users with email alerts and CSV logs	git clone https://github.com/misiektoja/instagram_monitor.git
Intelligence X (intelx.io)	Selective archive search — emails, leaks, paste sites, dark-web	intelx.io
Interlace	Easily turn single-threaded CLI apps into multi-threaded jobs	git clone https://github.com/codingo/Interlace.git
Joe Sandbox	Deep automated malware analysis (free tier)	joesandbox.com
JSFinder	Find JS files referenced from a URL — endpoints / API paths	git clone https://github.com/Threezh1/JSFinder.git
Kagi Search	Premium privacy-respecting search engine, no ads, no tracking	kagi.com
knock	Domain knock — security testing via DNS	git clone https://github.com/guelfoweb/knock.git
Knockpy	Subdomain enumeration scan with virtual host discovery	pip3 install knock-subdomains
linkedin2username	Generate usernames from a target's LinkedIn employees	git clone https://github.com/initstring/linkedin2username.git
LinkedInDumper	Dump/scrape company employees from LinkedIn API	git clone https://github.com/l4rm4nd/LinkedInDumper.git
Malpedia	Threat-actor groups, malware families, and analysis by Fraunhofer	malpedia.caad.fkie.fraunhofer.de
MalShare	Free malware sample repository for researchers	malshare.com
massdns	High-performance DNS stub resolver for bulk lookups	git clone https://github.com/blechschmidt/massdns.git
meg	Fetch many paths for many hosts without flooding	go install github.com/tomnomnom/meg@latest
Memento Time Travel	Federated search across multiple web archives	timetravel.mementoweb.org
Metadata2Go	Free online metadata extractor for any file	metadata2go.com
MetaDefender Cloud	Multi-engine file/URL/IP scanning by OPSWAT	metadefender.com
MetaSleuth	Free + paid crypto transaction tracing tool	metasleuth.io
MISP Galaxy	Adversary group identification used by SOCs/ISACs	misp-galaxy.org
Mitaka	Browser extension for OSINT — extract IoCs from highlighted text	git clone https://github.com/ninoseki/mitaka.git
Mnemonic Passive DNS	Free passive-DNS query tool	passivedns.mnemonic.no
Mojeek	Independent search engine that doesn't track users	mojeek.com
Mylnikov Geolocation	BSSID/Wi-Fi MAC to coordinates lookup	mylnikov.org
Naabu	Fast Go-based port scanner from ProjectDiscovery	go install github.com/projectdiscovery/naabu/v2/cmd/naabu@latest
Name Checkr	Check domain and username across many platforms	namecheckr.com
Name Checkup	Check username availability across social media	namecheckup.com
NameKetchup	Check domain + username on popular social media	nameketchup.com
Naver	South Korean search engine — local content not on Google	naver.com
NerdyData	Search engine for source code across the public web	nerdydata.com
Netcraft Site Report	Web technology, hosting history, takedown service	sitereport.netcraft.com
Oblivion	OSINT framework	git clone https://github.com/loseys/Oblivion.git
ODIN	Search hosts, CVEs, exposed buckets — 10 free searches/day	search.odin.io
Offshore Leaks Database	Panama/Pandora/Paradise Papers searchable database	offshoreleaks.icij.org
OnionLand Search	Search engine for dark-web content	onionlandsearchengine.com
Open-Source Intelligence (Reverse Image)	Yandex/Bing/TinEye combined reverse-image search	oosint.com
OpenCellID	Largest public database of cell-tower IDs	opencellid.org
opencorporates-cli	Command-line client for OpenCorporates API	pip3 install opencorporates
OpenPhish	Live phishing URL feed	openphish.com
OpenRailwayMap	Worldwide rail network map — rolling stock, infrastructure, signals	openrailwaymap.org
OpenSanctions	Consolidated database of sanctioned entities across 200+ sources	opensanctions.org
OXT (OpenXt)	Bitcoin transaction graph explorer with clustering	oxt.me
PassiveTotal (RiskIQ)	Passive DNS, WHOIS, SSL cert pivots — now Microsoft Defender TI	community.riskiq.com
Peekalink	Preview any URL — title, description, screenshot via API	peekalink.io
PhishStats	Live phishing intelligence feed and search	phishstats.info
PhishTank	Anti-phishing community — verified phishing URLs	phishtank.org
Picarta.ai	AI-powered photo geolocation predictor	picarta.ai
Pinterest	Visual search engine — alternate reverse-image source	pinterest.com
PolygonScan	Polygon (Matic) blockchain explorer	polygonscan.com
Predicta Search	Search social accounts by email or phone	predictasearch.com
Public Transport Maps	20+ online public transport maps by country	cipher387.github.io
PublicWWW	Search the web's source code (HTML/JS/CSS) for snippets, trackers, scripts	publicwww.com
PullPush	Index/retrieval service for Reddit (incl. deleted content)	pullpush.io
Pushshift API	Historical Reddit data — posts, comments, metadata	pushshift.io
Quake (360.cn)	Chinese internet asset search engine	quake.360.net
RECAP Archive	Public archive of PACER court documents	courtlistener.com
reconFTW	Full-suite domain recon — subdomain enum, port scan, vuln scan in one pipeline	git clone https://github.com/six2dez/reconftw.git
RedditMetis	Reddit user analysis — summary, top posts, activity stats	redditmetis.com
RedditSearch.io	Search archived Reddit content via Pushshift mirror	redditsearch.io
Revealer.cc	Discord-based account-checker & breach lookup	revealer.cc
RocketReach	Find professional emails/phones for 700M+ profiles	rocketreach.co
RustScan	Modern port scanner — finds open ports, then pipes to Nmap	git clone https://github.com/RustScan/RustScan.git
ScamAdviser	Check website trustworthiness scores	scamadviser.com
Scribd	Search for documents, presentations, sheet music, ebooks	scribd.com
searchcode	Search 75+ billion lines of public source code across GitHub/GitLab/Bitbucket	searchcode.com
Seeker	Geolocation by phishing — collects precise GPS via WebRTC + browser geolocation	git clone https://github.com/thewhiteh4t/seeker.git
Shadowserver Dashboard	Global statistics on cyber threats by Shadowserver Foundation	dashboard.shadowserver.org
Sherloq	Open-source image forensics toolset	git clone https://github.com/GuidoBartoli/sherloq.git
Shodan CLI	Official Shodan command-line client	pip3 install shodan
SlideShare	Search public PowerPoint/PDF presentations	slideshare.net
smap	Drop-in replacement for nmap powered by shodan.io	go install github.com/s0md3v/smap/cmd/smap@latest
Snusbase API	API access to breach data (premium)	snusbase.com
SourceGraph	Search code from millions of open-source repos	sourcegraph.com
SpyCloud	Account-takeover prevention + identity exposure data	spycloud.com
Startpage	Privacy-focused search — Google results with no tracking	startpage.com
StealSeek	Search engine for finding and analyzing data breaches	stealseek.io
SubredditStats	Subreddit user-overlap, growth, top posts	subredditstats.com
Telegago	Google CSE for finding public/private Telegram channels	cse.google.com
Telegram Nearby Map	Find positions of nearby Telegram users via OSM	git clone https://github.com/tejado/telegram-nearby-map.git
Telegram Search (lyzem.com)	Search public Telegram messages and channels	lyzem.com
Telemetr	Telegram channel/group analytics	telemetr.io
Telerecon	Reconnaissance framework for investigating Telegram	git clone https://github.com/sockysec/Telerecon.git
Teleteg	Telegram search engine — 10 free results	teleteg.com
TGStat	Telegram channel analytics — post stats, audience overlap	tgstat.com
The Hidden Wiki	Curated directory of dark-web sites (mirror-dependent)	thehiddenwiki.org
the-endorser	Map LinkedIn endorsements/skills to draw out person relationships	git clone https://github.com/eth0izzle/the-endorser.git
TikTok Finder Country	Free OSINT lookup for TikTok account country/language	tiktokfindercountry.xyz
TorghostNG	Anonymize all OS traffic via Tor (Linux)	git clone https://github.com/githacktools/TorghostNG.git
TOsint	Extract info from Telegram bots and channels	git clone https://github.com/drego85/tosint.git
Trace	Search usernames, emails, phones across 600+ platforms with risk scoring	trace.manus.space
Transit Visualisation Client	Real-time public transport across 700+ cities	tracker.geops.ch
Trends24	Twitter trends history per country	trends24.in
TRM Labs	Crypto compliance and investigation platform	trmlabs.com
TweetBinder	Twitter/X analytics dashboards	tweetbinder.com
Twitch Search	Search live streams by category, language, viewer count	twitch.tv
Twiteur	Twitter/X advanced search wrapper — geo, date, sentiment	twiteur.com
U-Find	Reddit user comment / submission scraper	u-find.com
uncover	ProjectDiscovery — quickly find exposed hosts via Shodan/Censys/Fofa	go install github.com/projectdiscovery/uncover/cmd/uncover@latest
URLCrazy	Generate domain typos and check availability/registration	git clone https://github.com/urbanadventurer/urlcrazy.git
URLhaus (abuse.ch)	Database of malicious URLs used for malware distribution	urlhaus.abuse.ch
User-Searcher	Search a username across 2000+ websites	user-searcher.com
Vehicle Number Search Toolbox	Search 14 country license plates from one page	cipher387.github.io
Venacus	Search for your data breaches and get notified when compromised	venacus.com
Vigilante.pw	Index of dumped databases (educational)	vigilante.pw
VMRay Analyzer	Malware sandbox analysis platform	vmray.com
WalletExplorer	Smart bitcoin block explorer — clusters addresses by entity	walletexplorer.com
waybackurls	Fetch all URLs the Wayback Machine knows about a domain	go install github.com/tomnomnom/waybackurls@latest
Whoisology	Reverse WHOIS — find domains by registrant	whoisology.com
Whoxy	WHOIS lookup with reverse-WHOIS, history, and bulk API	whoxy.com
Wikidata	Wikipedia's structured-data backbone — query via SPARQL	wikidata.org
Wikipedia	Free encyclopedia — start of every people/place investigation	en.wikipedia.org
WorldLicensePlates	Graphic index of license plates by country	worldlicenseplates.com
XeuleDoc	Fetch info on Google Docs/Sheets/Slides/Drawings without auth	pip3 install xeuledoc
Yandex	Russian search engine — strong reverse-image and Cyrillic support	yandex.com
YARAify	Collaborative YARA engine for open threat intel via file pattern matching	yaraify.abuse.ch
Yumpu	Document publishing — sometimes leaks via search	yumpu.com
ZeroBounce	Email validation and deliverability service	zerobounce.net
ZoomEye CLI	Command-line interface for ZoomEye internet asset search	pip3 install zoomeye
50. 🇬🇪 Georgian OSINT Arsenal (500+ resources)
🇬🇪 The most comprehensive OSINT resource collection for the country of Georgia (Sakartvelo).

28 sub-sections · 500+ verified resources — government databases, public registries, investigative tools, open-data portals, Telegram bots & more.

Pro tip: Pair this with my Georgian-Wordlist (760K Georgian words for security research) and Wordlist-Generator.

Warning

Educational and lawful investigative use only. Respect Georgia's Law on Personal Data Protection and the GDPR. Authors are not responsible for any misuse.

📋 Click to expand the full Georgian OSINT Arsenal (28 sub-sections)
🤝 Contributing & Issues
Found a dead link? Tool that should be here? Just open an issue or PR.

Found something broken → open an issue
Want to add a tool → fork, add it to the right section in alphabetical order, PR
No time to PR? → leave the tool name + URL in an issue, I'll add it
Verify install commands on a fresh Kali VM before submitting.

⚖️ Legal Disclaimer
This repository is provided for educational and authorized security research purposes only.

✅ Legal uses:

Security research on systems you own
Penetration testing with written authorization
OSINT for journalism or missing persons investigations
Bug bounty programs with defined scope
Security awareness training
❌ Illegal uses (never do these):

Unauthorized access to systems or accounts
Stalking or harassment
Credential theft
DDoS or attacks on systems you don't own
Privacy violations
Laws that apply: GDPR (EU), CCPA (California), CFAA (US), Computer Misuse Act (UK), and your local equivalents. Know your laws before you act.

The maintainers of this repository are not responsible for any misuse of information or tools listed here.


Built for the OSINT and security research community.

Knowledge is power — use it responsibly.

Buy Me a Coffee


⭐ Star this repo if you found it useful!

GitHub stars GitHub forks


About
🔍 Curated OSINT & recon toolkit for Kali Linux — 100+ tools, one-command installer, covering SOCMINT, GEOINT, network recon, dark web, forensics & more.

Topics
intelligence osint hacking open-data cybersecurity penetration-testing infosec recon kali-linux ethical-hacking information-gathering security-tools investigation reconnaissance data-breach goverment-data public-records osint-tool osint-tools
Resources
 Readme
 Activity
Stars
 1.3k stars
Watchers
 9 watching
Forks
 214 forks
Report repository
Releases
No releases published
Packages
No packages published
Contributors
3
@rawfilejson
rawfilejson barni
@kriptoburak
kriptoburak Burak Bayır
@Salzling
Salzling Salzling
Languages
Shell
100.0%
Footer
© 2026 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Community
Docs
Contact
Manage cookies
Do not share my personal information
