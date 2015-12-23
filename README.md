**Login**
----
  
  Number26 uses a very straight-forward HTTP-Header authentication mechanism using JSON Web Token (JWT). You send your credentials to their backend and receive a JWT as a response which you have to send along with any further requests.
  
* **URL**

  https://api.tech26.de/oauth/token

* **Method:**
  
  `POST`

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

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._> 
