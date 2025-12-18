
Objective : Reset Morty's password via the Forgot Password mechanism with _his obfuscated answer_ to his security question

methodology : 

	Tools used :  Burp (Proxy,HTTP history,Intruder) PrudoHash

	1. The first step is to find the answer to his security question. The question is “What is the name of his favorite animal?” Having seen the series, I know that his favorite animal is his dog named Croquette, but whose name has been changed to Snowball.

	2. So we have the answer, but now we need to encrypt it in several ways. I used PsudoHash to obtain a text file with a wide variation of “Swonball.”

	3. On the website, we need to obtain the request. To do this, we need to go to “Forgot Password,” try to answer the question, and change the password.  

	4. Now, in the HTTP history, we need to copy the request with “forgot-password” in the URL and go to Intruder on Burp.

	5. In Intruder, we load the payload with the Load button and in the request, we use the Add button to choose where we want to test the response.

	6. Then lauch Attack.
	
vulnerabilities :

	Vulnerability type : Broken Anti Automation

	Affected compnonent : 
		Password recovery feature    
		Security question system

	Estimated severity : High
		Because attackers can reset user's password account and then get user's account 

risks :

	Account takeover : An attacker could reset the password of a user whose recovery answer is trivial or publicly known

	Loss of confidentiality : Unauthorized access to personal data, shopping history, or sensitive account information.

actions :

	Remove or harden security questions :  Avoid predictable questions
    
	Use secure password-reset feature : Sent by email link to reset password

	Implement try limit : Limit the number of password recovery attemps per IP

	Add CAPTCHA protection : Prevent automated attacks 