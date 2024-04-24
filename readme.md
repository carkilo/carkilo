Create a website.
Get website parked url.
Clone homepage html.
Modify the html to redirect to the parked url. (e.g): 

-create a git repository and add the html to it
-go to the github.pages and publish the website

-go to the dns management and add the following records.
* CNAME Record for www:
  Type: CNAME
  name: www
  Value: carkilo.github.io
  TTL: 1 Hour
  Make sure that this CNAME record is added correctly. The Name should be www and the Value should be carkilo.github.io.

* A Records for @ (root domain):
  You've already added the A records for the root domain (@). Now, ensure they are correctly added and propagated:
  
  Type: A
  Name: @
  Value: 185.199.108.153
  TTL: 1 Hour
  Type: A
  Name: @
  Value: 185.199.109.153
  TTL: 1 Hour
  Type: A
  Name: @
  Value: 185.199.110.153
  TTL: 1 Hour
  Type: A
  Name: @
  Value: 185.199.111.153
  TTL: 1 Hour

check the dns status using https://www.nslookup.io/.


Go to the github pages and add the custom domain (e.g): carkilo.com

if all the steps followed correctly, you should be able to view your website at www.carkilo.com and carkilo.com. (bith will point to the website parked url)

thus, you'll get your website deployed for free.

மகிழ்ந்திடு ! 
