Features
	•	Host discovery (TCP sweep) — probes a host or subnet on common ports to find live hosts
	•	Port scanning — multi-threaded TCP connect scan over a single port, list, or range
	•	Banner grabbing — captures service banners on open ports
	•	Service fingerprinting — basic detection of SSH, HTTP, SMTP, FTP, MySQL, SMB, RDP, VNC, UPnP from banner text
	•	TLS inspection — pulls certificate CN, SANs, issuer, and days-until-expiry on HTTPS ports
	•	HTTP enumeration — fetches the root page, title, server headers, robots.txt, and checks a short list of common admin paths (non-intrusive, GET requests only)
	•	Passive vulnerability triage — flags things like exposed DB/SMB ports or anonymous FTP banners; does not attempt logins, exploits, or brute force
	•	Optional CVE lookups — queries the NVD API by detected product/version (requires the requests library and, for higher rate limits, an NVD API key)
	•	JSON + CSV reporting — saves a full report of every finding per run
	•	Interactive or non-interactive — run it with guided prompts, or fully scripted via CLI flags or a JSON config file
Requirements
	•	Python 3.7+
	•	Optional: requests — only needed for NVD CVE lookups; the tool runs fine without it, it just skips that step