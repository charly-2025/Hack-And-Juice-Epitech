methodology : 
	tools used :  Burp
	
	act as if we wanted to buy an object then go to the console and see in the main.js file and look by doing crl + f discount and take one of the codes and measure their PC on that date and enter the promo code then proceed to buy it

	-Analysis of the logic of coupons

	-Test of expired coupons

	-Interception of validation requests

	-Modification of dates or states

vulnerabilities :

	-Poor management of the expiration date

	-Client-side validation only

risks :

	-Use of expired coupons

	-Financial loss

actions :

	-Interception of the coupon application request

	-Modification of the date or status

	-Sending the modified request

	-Expired coupon accepted