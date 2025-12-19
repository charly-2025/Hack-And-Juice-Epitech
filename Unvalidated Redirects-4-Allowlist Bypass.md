
methodology : 

	1. To redirect to an unauthorized page, put this "https://ctf.juice.cyber.epitest.eu/redirect?to=https://google.com/https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm" in the url

	2. You can put whatever you want in place of google.com, the most important thing is to keep the blockchain link at the end because it allows you to bypass the whitelist.

	3. Actually, if we enter google.com, it blocks us, but if we add an authorized URL at the end, the site sees it and only retains the authorized URL and ignores the rest.

vulnerabilities :

	Vulnerability type : Unvalidated Redirect – Allowlist Bypass
		
	Affected compnonent : 
		Redirect mechanism
		
	Estimated severity : High
		Because attackers can redirect users to molicious websites

risks :

	Phising attacks : Users can be redirected to fake login pages

	Malware distribution : The attacker can redirect to a virus installer

actions :

	Implement strict allowlist : Compare the authorized redirect URL and the final redirect URL.