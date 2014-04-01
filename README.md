# Oauth2 #

A CFC for Oauth2. 

# Getting Started #

To get started, fill in your own client_id, client_secret and scope.  These are found in the Google developer console.  Make the changes in application.cfc.  

```
	<cfset application.oauth2 = new oauth2.oauth2(
		client_id 		=   'YOUR %Client ID%',
		client_secret 	= 	'YOUR %Client secret%',
		redirect_uri	=	'http://localhost/GoogleCal/oauth2/index.cfm',
		scope           =   'https://www.googleapis.com/auth/calendar',
		state			=	'',
		access_type		=	'offline', <!--- Use offline for refresh tokens --->
		approval_prompt	=	'force'
	) />
```

Contributors:

Author: William Eatman @billeatman
   
Based on Oauth2 work done by Matt Gifford @coldfumonkeh
http://googleanalytics.riaforge.org/
