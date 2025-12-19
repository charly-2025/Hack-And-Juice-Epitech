
Objective : Obtain a Deluxe Membership without paying for it.

methodology : 

	Tool used : Burp (Proxy/intercept)

	1. Create a new account and login if necessary 

	2. Go to Deluxe Membership page and click to become a member add a new card

	3. Before click on Continue, launch on Burp Intercept and click on Continue

	4. In the request remove the body and forward the request 

vulnerabilities:

    Vulnerability type : Improper Input Validation – Client-Side Validation Bypass

    Affected component :
        Payment process
        Membership validation mechanism

    Estimated severity : High
        Because users allows to gain paid privileges without completing a valid payment

risks:

    Financial loss : Attackers can obtain premium features without paying

    Unfair access : Non-paying users gain advantages over legitimate customers

    Business impact : Loss of revenue and reduced trust in the platform’s payment system

actions:

	Payment method verification: Ensure that the payment method is correctly specified and valid in the request.
