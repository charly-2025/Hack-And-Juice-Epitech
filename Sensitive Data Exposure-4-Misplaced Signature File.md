
Objective : Access a misplaced SIEM signature file.

methodology : 

	1. The first step is to access the confidential documents page.

	2. When we click on suspicious_errors.yml, we get an error because only .md and .pdf formats are allowed.

	3. Since we couldn't open the file on the website, I tried to download it. But that's not allowed either.

	4. The solution is therefore to download the file, but in .md format. To obtain the file, simply click on it and add “%2500.md” to the URL. On the FTP page, you can add “suspicious_errors.yml%2500.md” to the URL.

vulnerabilities :

	Vulnerability type : Sensitive Data Exposure – Unprotected Internal File
		
	Affected compnonent : 
		Web server file
		
	Estimated severity : High
		Because attackers can retrieve sensitive information without authentification

risks :

	Leak of sensitive infomation
	Application compromise if leaked data is reused by an attacker

actions :

	Disable access to sensitive path 