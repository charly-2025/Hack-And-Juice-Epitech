methodology : 
	tools used :  Burp
	
	1-Apply an expired coupon.

	2-Intercept the request.
	
	3-Change the date or status of the coupon.
	
	4-Send the request.
	
	5-Check the acceptance of the coupon.
	
	Techniques used: Manipulation of parameters
	Tools: Burp Suite

vulnerabilities :

	Poor management of business logic
	Severity: Average
risks :

	Use of expired coupons
	Financial loss
actions :

	Server verification of dates