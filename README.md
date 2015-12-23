**Login**
----
  
  Number26 uses a very straight-forward HTTP-Header authentication mechanism using JSON Web Token (JWT). You send your credentials to their backend and receive a JWT as a response which you have to send along with any further requests.
  
* **URL**

  https://api.tech26.de/oauth/token

* **Method:**
  
  `POST`

* **Request Header**
 
  `Host: api.tech26.de`

  `Connection: keep-alive`

  `Content-Length: 76`

  `Accept: application/json, text/javascript, */*; q=0.01`

  `Origin: https://my.number26.de`

  `User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.106 Safari/537.36`

  `Authorization: Basic bXktdHJ1c3RlZC13ZHBDbGllbnQ6c2VjcmV0`

  `Content-Type: application/x-www-form-urlencoded`

  `Referer: https://my.number26.de/`

  `Accept-Encoding: gzip, deflate`

  `Accept-Language: de-DE,de;q=0.8,en-US;q=0.6,en;q=0.4`


* **Data Params**

  `grant_type = password`
  
  `username = mail@example.com`
  
  `password = examplepassword`
  

* **Success Response:**

  * **Code:** 200
  * 
    **Content:** `{
  "access_token": "eyJhbGciOiJIUzI1NiJ9.eyJleHAiOjE0NTA4OTc1OTAsInVzZXJfbmFtZSI6Im1lQGV4YW1wbGUuY29tIiwiYXV0aG9yaXRpZXMiOlsiVVNFUiJdLCJqdGkiOiIxMjNhMTJiYy0xYWJjLTFhMTItMTJhYi0xMjNhMTJhMTJhYjEiLCJjbGllbnRfaWQiOiJteS10cnVzdGVkLXdkcENsaWVudCIsInNjb3BlIjpbInJlYWQiLCJ3cml0ZSIsInRydXN0Il19.KN7RvK7DW_yPcO-D6Oz6-cq5zBIaaGYVyApsUSqEyZ0",
  "token_type": "bearer",
  "expires_in": 1799,
  "scope": "read write trust",
  "jti": "123a12bc-1abc-1a12-12ab-123a12a12ab1"
}`
