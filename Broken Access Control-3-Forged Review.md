
methodology : 

	Tools used : Burp (Proxy,Intercept)
	
	1. The first step is to launch the site, write a review on a product, and then prepare to send it.
	
	2. Just before sending it, activate Burp interception to retrieve the request.

	3. Now send it. Once retrieved, change the author to the email of the user you want and that exists, and finally send the request back.

vulnerabilities :

	Tulnerability type : Broken Acces Control - Insercure Direct Object Reference

	Affected compnonent : 
		Review
		Database storing users'reviews

	Estimated severity : High
		Because attackers can put what they want

risks :

	User identity theft : Attackers can make a review with any identity

	Reputation damage : Fake reviews harm the platform's credibility

	Loss of customer trust : Manipuling product review impacts customer perception

actions :

	Remove author field from the request : The author must be determined by the server