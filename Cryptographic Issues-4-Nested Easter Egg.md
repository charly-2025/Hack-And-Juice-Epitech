
methodology : 

	Tool used : Base64 decoder, Caesar cipher deocoder

	1. Open the easter egg file and copy the base64 encoded line
	
	2. Decode the base64 line whith Base64 decoder and after decode the result in Caesar cipher decoder
	
	3. Finally, paste the result : "/the/devs/are/so/funny/they/hid/an/easter/egg/within/the/easter/egg", at the last of web url

vulnerabilities :

	Vulnerability type : Cryptographic Issues - Use of Weak Encoding
	
	Affected compnonent : 
		Easter Egg File
		Encoding layer used to hide sensitive paths

	Estimated severity : Low
		Because the challenge doesn't expose sensitive data

risks :

	Exposure of internal paths or development traces : Attackers can discover unintended routes, comments, or development artifacts.

actions :

	Remove unnecessary internal routes : Hidden paths should not be accessible
    
	Apply proper cryptographic practices : Use modern methods