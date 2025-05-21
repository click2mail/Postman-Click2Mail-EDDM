# Postman-Click2Mail-EDDM
To create and submit an EDDM job via APIs, call the following APIs:

Upload the document:
POST https://stage-rest.click2mail.com/molpro/documents 
Documentation:
https://developers.click2mail.com/reference/createdocument_1 

Create the job:
POST https://stage-rest.click2mail.com/molpro/jobs 
Documentation:
https://developers.click2mail.com/reference/post_2 

Specify EDDM mailer's info:
POST https://stage-rest.click2mail.com/molpro/jobs/{id}/eddmInfo 
Documentation:
https://developers.click2mail.com/reference/updateeddminfo 

Specify the EDDM Post Office (where the mail will be submitted):
POST https://stage-rest.click2mail.com/molpro/jobs/{id}/eddmPo 
Documentation:
https://developers.click2mail.com/reference/updateeddmpo 

Specify the EDDDM routes. This API will be called multiple times, once for each route.
POST https://stage-rest.click2mail.com/molpro/jobs/{id}/eddmRoute 
Documentation:
https://developers.click2mail.com/reference/updateeddmroute 

(optional): Generate a proof of the job:
POST https://stage-rest.click2mail.com/molpro/jobs/{id}/proof 
Documentation:
https://developers.click2mail.com/reference/createproof 

(optional): Accept the proof
POST https://stage-rest.click2mail.com/molpro/jobs/{id}/proof/accept 
Documentation:
https://developers.click2mail.com/reference/acceptproof 

(optional): Get the job cost:
GET https://stage-rest.click2mail.com/molpro/jobs/{id}/cost 
Documentation:
https://developers.click2mail.com/reference/getjobcost 

Submit the job:
POST https://stage-rest.click2mail.com/molpro/jobs/{id}/submit 
Documentation:
https://developers.click2mail.com/reference/submitjob 

(optional): Get the status of the job:
GET https://stage-rest.click2mail.com/molpro/jobs/{id} 
Documentation:
https://developers.click2mail.com/reference/getjob 
