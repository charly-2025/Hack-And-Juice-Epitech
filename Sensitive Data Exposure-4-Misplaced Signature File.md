
methodology : 

	1. For get Backup you have to put this : "ftp/suspicious_errors.yml%2500.md" in the url after the source url of your website 

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