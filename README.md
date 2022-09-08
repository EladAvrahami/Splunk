<pre>           </pre>     <img src="https://upload.wikimedia.org/wikipedia/commons/e/e8/Splunk-Logo.jpg" alt="" width="800" height="300"> 


# Splunk
<pre>
https://www.splunk.com/pdfs/training/Splunk-Education-Student-Handbook.pdf
https://education.splunk.com/free
https://www.splunk.com/en_us/resources/videos/create-dashboard-in-splunk-enterprise.html
SPL -SPLUNK LANGUAGE : https://docs.splunk.com/Documentation/SplunkCloud/latest/Search/Aboutthesearchlanguage
learn for free:https://education.splunk.com/single-subject-courses?_ga=2.25519290.660583283.1644217651-1092567743.1640770338
splunk command Doc : https://docs.splunk.com/Documentation
splunk elerning videos: https://education.splunk.com/single-subject-courses?_ga=2.25519290.660583283.1644217651-1092567743.1640770338
learn Splunk command youtube: https://www.youtube.com/c/SiddharthaChakraborty/search?query=Splunk%20Commands

splunk elerning by Topic https://www.splunk.com/en_us/training.html?sort=Newest

youtube practical courses using splunk & ML : https://www.youtube.com/c/SiddharthaChakraborty
https://www.youtube.com/watch?v=k3pO0B7C1Hk

</pre>

<h3>basic search commands : </h3>
<pre>
 
build table and reaname colomn :
|table feildname1 feildname2 feildname3  | rename feildname1 as nomatterwhatname  feildname2 as anothename

build table and dont show one colomn:
|table feildname1 feildname2 feildname3  | fields - feildname1 

build table and Makes columns show only unique values  :
|table feildname1 feildname2 feildname3  |  dedup feildname1 

build table and Makes columns show by a-z  :
|table feildname1 feildname2 feildname3  |  sort  feildname1  

build table and Makes columns show by z-a  :
|table feildname1 feildname2 feildname3  |  sort  - feildname1 

</pre>

js liborary that implimant charts and graphs - https://apexcharts.com/


https://drive.google.com/file/d/15OfNgGpVqJf_imiwYix-dRepwxMlbICT/view הרצאה בעברית על הכלי 



<h3> searches commands</h3>
<pre>
build table and reaname colomn :
|table feildname1 feildname2 feildname3  | rename feildname1 as nomatterwhatname  feildname2 as anothename

build table and dont show one colomn:
|table feildname1 feildname2 feildname3  | fields - feildname1 

build table and Makes columns show only unique values  :
|table feildname1 feildname2 feildname3  |  dedup feildname1 

build table and Makes columns show by a-z  :
|table feildname1 feildname2 feildname3  |  sort  feildname1  

build table and Makes columns show by z-a  :
|table feildname1 feildname2 feildname3  |  sort  - feildname1  



```this is how you write command in splunk apig_appl_40620``` 
```use shift+enter to drop line```
index=apig_appl_40620  "fault": "GatewayTimeout"
| timechart count as


מראה את כל השגיאות באפיגי לפי חודש 
index=apig_appl_40620  "fault.name" !=""
| timechart count as Failures


מראה שגיאות באפיגי לפי סוג השגיאה 
index=apig_appl_40620  "fault.name" !=""
| chart count  over fault.name

כמו הקודם +נותן שם לעמודה 
index=apig_appl_40620  "fault.name" !=""
| chart count as Failures over fault.name





התוצאות תלויות בסדר שהאירועים מגיעים -centralized streaming commnads
|transaction
|streamstats
התוצאות לא תלויות במשהו ואין סדר אירועים (מהיר יותר ) - distributedble streaming commands
|rename
|eval
|fields
| regex

Segmentation - tokenized search terms at search time
חיפוש של משהו 
למשל 
index=apigee "failed password" יחפש או את המילה נכשל או את המילה סיסמא 
במידה ואני רוצה לחפש איזושהיא מילה או כתובת איפי שיש בין המס או אותיות רווחים או סימנים מיוחדים אשתמש ב TREM 
למשל:
index=apigee  clientip=TREM(76.160.176.252) מחפש את הסטרינג המדוייק ולא 76 או 160 בנפרד למל 



</pre>
