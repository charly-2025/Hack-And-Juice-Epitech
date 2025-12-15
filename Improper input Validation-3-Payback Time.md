methodology : 
	tools used :  Burp
	
	add an object to retrieve on burp in the http history the post that was made, copy and paste this request into the repeater then change the productid to number 33 and set the quantity to –1000 then send the request and we will see a negative payment in our cart and subsequently buy it
	-Analysis of the business logic related to reimbursement

	-Interception of requests with Burp Suite

	-Identification of the parameters controlling the amount or time

	-Modification of the values sent to the server

	-Observation of application behavior
	
vulnerabilities :

	-Insufficient validation of business parameters

	-Lack of server control over critical values

risks :

	-Financial manipulation

	-Fraud or illegitimate refund

	-Financial loss for the company

actions :

	-Interception of the refund request

	-Modification of parameters related to amount / timing

	-Sending the modified request

	-Unauthorized refund validation