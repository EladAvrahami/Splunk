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
