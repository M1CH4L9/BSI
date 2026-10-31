## h 3.1 p
```bash
#Open http://192.168.100.153/ in website
#Go to Burp and right click '/' URL and select 'Send to Repeater'
#Change 'Cookie: debug=false' to true
```

## h 3.2 p
```bash
#Open http://192.168.100.153/login/ in browser
#Go to Burp and right click '/login/' URL and select 'Send to Repeater'
#Change 'Cookie: debug=false' to 'Cookie: debug=true'
#Change 'GET /login/' to 'GET /usersdata/' and click 'Send'
```

## h 3.3 p
```bash
#Open http://192.168.100.153/login/ in browser
#Go to Burp and right click '/login/' URL and select 'Send to Intruder'
#Change 'GET /login/' to 'GET /usersdata/4/' and 'Cookie: debug=false' to true
#Select '4' and click 'Add §' (should be /usersdata/§4§/)
#On the right set 'Payload type' to 'Numbers', From: 1, To: 50, Step: 1
#Click 'Start attack'
```

## h 3.4 p
```bash
#Find Hacker in Intruder results (payload 48)
#Copy the encoded data from Hacker's response
#Go to Burp -> Decoder, paste it and select 'Decode as...' -> 'Base64'
#Copy the decoded URL and paste it into Repeater (GET /h4ck3r1333733x/)
#Keep 'Cookie: debug=true' and click 'Send'
```

## h 3.1
```bash

```
