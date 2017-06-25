
# getUserPosts

To get a list of Users posts

**URL:** *http://apigargoyle.com/GargoyleApi/beta/getUserPosts*
### Request Format
The getUserPosts API call can be refined by adding one or more of the following parameters

Parameter | Description
--------- | -----------
limit | Number of records to be retrieved. Default is 10 when limit not set. limit=0 returns all records
uid | user id of the user. Allows “=” behavior


```http
GET /getUserPosts HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getHackingItems",
  "message": "SUCCESS",
  "results": [
    {
      "postContent": "موضوع جميل شكرا لصاحب الموضوع لتقديم يد العون للأعضاءراجيا من بقية الاعضاء عدم الخروج عن نطاق الموضوعوشكرا مرة اخرى",
      "createdDate": "2017-05-30",
      "postedDate": "None",
      "forumsId": 72,
      "uid": 1,
      "boardsName": ":: hacker  منظمة قانون الهكر organization::",
      "postsId": 32671697
    }
  ]
}

```

* URL with single request parameter: To give a single parameter to a request, specify a parameter with its value like examples given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getUserPosts?limit=2*

2. *http://apigargoyle.com/GargoyleApi/beta/getUserPosts?uid=1*

* URL with multiple request parameters: To give multiple parameters to a request, separate each parameter with ‘&’ like the example given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getUserPosts?limit=3&order=uid*

### Response Format

Parameter | Description
--------- | -----------
type | Name of API call
message | status of the API call
results | List of user posts


** A sample response is shown on the right side **

