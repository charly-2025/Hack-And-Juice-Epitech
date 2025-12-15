methodology : 
	tools used :  Burp
	
	retrieve the post when we send a file and go to repeater and change the file into anything except pdf or zip

	-Analysis of the file upload mechanism

	-Testing client-side controls

	-Interception of the upload request

	-Modification of the MIME type and extension
	
vulnerabilities :

	-Absence of server validation of the file type

	-Control based on extension only

risks :

	-Upload malicious files

	-Execution of arbitrary code

	-Server compromise

actions :

	-Sélection d’un fichier interdit
    
	-Interception de la requête d’upload
    
	- Modification de l’extension / Content-Type
    
	- Upload accepté par le serveur