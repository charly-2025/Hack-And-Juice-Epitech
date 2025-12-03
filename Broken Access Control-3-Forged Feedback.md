
methodology : 

	tools used : Burp (Proxy,Intercept)
	
	1. The first step is to launch the site, write a review on a product, and then prepare to send it.
	
	2. Just before sending it, activate Burp interception to retrieve the request.

	3. Now send it. Once retrieved, change the user ID to the ID of the user you want and that exists, and finally send the request back.

vulnerabilities :

	vulnerability type : Broken Acces Control - Insercure Direct Object Reference

	affected compnonent : 
		Review/Feedback
		Database storing users'reviews

	estimated severity : High
		Because attackers can put what they want

risks :

	User identity theft : Attackers can make a review with any identity

	Reputation damage : Fake reviews harm the platform's credibility

	Loss of customer trust : Manipuling product feeback impacts customer perception

actions :

	Remove user ID field from the request : The user ID must be determined by the server