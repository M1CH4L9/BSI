## h 3.1 p
```bash
#Open http://192.168.100.153/ in website
#Go to Burp and right click '/' URL and select 'Send to Repeater'
#Change 'Cookie: debug=false' to true
```

## h 3.2 p - Przekierowanie
```bash
#On Kali open Burp Suite and http://192.168.100.153/login/ in browser
#Find GET /login/ in Burp, right click and select 'Send to Repeater'
#Click 'Send' and inspect the response body before following the redirect
#302 Found still contains HTML with 'Welcome admin!' and a link to /usersdata/
#In Repeater change the request path to GET /usersdata/ (keep Host: 192.168.100.153)
#Click 'Send' and inspect the response
#Open http://192.168.100.153/usersdata/ in browser
#Result: Users' Data - John, Henry, Maria, Pat, Mat
#BTW initial 408 timeouts disappeared after resetting the machine on the server
```

## h 3.1
```bash

```

## h 3.1
```bash

```

## h 3.1
```bash

```
