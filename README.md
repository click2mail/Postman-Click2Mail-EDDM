# Postman-Click2Mail-EDDM
To create and submit an EDDM job via APIs, call the following APIs:

Upload the document:
<br/>POST https://stage-rest.click2mail.com/molpro/documents 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/createdocument_1 
<br/>
<br/>Create the job:
<br/>POST https://stage-rest.click2mail.com/molpro/jobs 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/post_2 

<br/>Specify EDDM mailer's info:
<br/>POST https://stage-rest.click2mail.com/molpro/jobs/{id}/eddmInfo 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/updateeddminfo 
<br/>
<br/>Specify the EDDM Post Office (where the mail will be submitted):
<br/>POST https://stage-rest.click2mail.com/molpro/jobs/{id}/eddmPo 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/updateeddmpo 
<br/>
<br/>Specify the EDDDM routes. This API will be called multiple times, once for each route.
<br/>POST https://stage-rest.click2mail.com/molpro/jobs/{id}/eddmRoute 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/updateeddmroute 
<br/>
<br/>(optional): Generate a proof of the job:
<br/>POST https://stage-rest.click2mail.com/molpro/jobs/{id}/proof 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/createproof 
<br/>
<br/>(optional): Accept the proof
<br/>POST https://stage-rest.click2mail.com/molpro/jobs/{id}/proof/accept 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/acceptproof 
<br/>
<br/>(optional): Get the job cost:
<br/>GET https://stage-rest.click2mail.com/molpro/jobs/{id}/cost 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/getjobcost 
<br/>
<br/>Submit the job:
<br/>POST https://stage-rest.click2mail.com/molpro/jobs/{id}/submit 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/submitjob 
<br/>
<br/>(optional): Get the status of the job:
<br/>GET https://stage-rest.click2mail.com/molpro/jobs/{id} 
<br/>Documentation:
<br/>https://developers.click2mail.com/reference/getjob 
