c
methodology : 

	Tools used : Burp (Proxy,Intercept)
	
	1. The first step is to launch the site, write a feedback, and then prepare to send it.
	
	2. Just before sending it, activate Burp interception to retrieve the request.

	3. Now send it. Once retrieved, change the user ID to the ID of the user you want and that exists, and finally send the request back.

vulnerabilities :

	Vulnerability type : Broken Access Control - Insercure Direct Object Reference

	Affected compnonent : 
		Feedback
		Database storing feedback

	Estimated severity : High
		Because attackers can put what they want

risks :

	User identity theft : Attackers can make a feedback with any identity

	Reputation damage : Fake feedback harm the platform's credibility

	Loss of customer trust : Manipuling feeback impacts customer perception

actions :

	Remove user ID field from the request : The user ID must be determined by the server