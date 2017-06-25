# getHackingItems

To get a list of Hacking Items from various market places.

**URL:** *http://apigargoyle.com/GargoyleApi/beta/getHackingItems*
### Request Format
The getHackingItems API call can be refined by adding one or more of the following parameters.

```http
GET /getHackingItems HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getHackingItems",
  "results": [
    {
     “autoTranslated”: false,
      "itemId": 973846,
      "itemName": " [may 2017] coinbase- payoneer - bank transfer - western union-- mega cashout guide. [$12,590.",
      "itemDescription": "[$12,590.00 value - next 10 pay $10]\n\n???????? four ultimate and personal private guides ????????\n\n\nguide 1 ??? coinbase (coinbase.com) - [may 2017 update] ??? ",
      "language": "English",
      "uid": "68075",
      "marketplaceId": "6",
      "recordedTime": "12:00:00",
      "scrapedDate": "2017-06-05",
      "postedDate": "None",
      "recordedDate": "2017-06-05",
      "itemCve": null,
      "itemMs": null,
      "itemCategory": null,
      "itemEscrowinfo": null,
      "itemViews": null,
      "itemLastViewDate": "None",
      "itemQuantitySold": null,
      "itemQuantityLeft": 82,
      "itemShippedFrom": null,
      "itemShippedTo": null,
      "itemVendorRating": "93.42",
      "itemSuccessfulTrans": "100.00",
      "softwareTags": null,
      "financialTags": null,
      "entity": [
        {
          "entityId": "2",
          "freebaseTypes": null,
          "type": [
            "Duration"
          ],
          "matchedText": "2 weeks",
          "entityEnglishId": ""
        },
      "sellingPrice": [
        {
          "sellingPriceUsd": "12.000000"
        }
      ],
      "tags": null
    }
  ],
  "message": "SUCCESS"
}

```

Parameter | Description
--------- | -----------
start | start record of the results that is to be retrieved. Default is 0 when start is not set. Allows “=” behavior
limit | Number of records to be retrieved. Default is 10 when limit not set. Maximum limit is 10000. When more data having index > 10000 is to be retrieved set start=10000 and limit = "some amount of results you want"
itemName | Name of product to be retrieved; allows “Like” behavior, so any searched pattern contained w/in itemName will return records
itemId | itemId of the Item. Allows “=” behavior
startPrice | 
endPrice | 
nullPrice |
language | language of the product listing; behavior is “=” to match exact language (list of valid languages below, CASE sensitive, some languages return 0 records). Multiple language names can be given with '\|' as the separator. Languages can be Arabic, Chinese, English, French, German, Italian, Japanese, Mandarin, Persian, Polish, Portuguese, Russian, Swedish, Vietnamese
desc | Any text pattern; allows “Like” behavior, so any searched pattern contained w/in a product name or description will return records
uid | user id of the user. Allows “=” behavior
pastDay |
order | sorts the records according to the parameter in descending order. The default order parameter is recorded_date
itemCategory | Name of the category that items are classified into. Multiple item categories can be given with "|" as the separator
getCount | if set to true, it will return the total number of results with the filters in place.
from | Date (YYYY-MM-DD) from which information was scraped; if “to” is not specified, then information through the present is returned
to | Date (YYYY-MM-DD) to which information was scraped; if “from” is not specified, then information starting from the earliest available in the dB is returned

* URL with single request parameter: To give a single parameter to a request, specify a parameter with its value like examples given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getHackingItems?itemName=coin*

2. *http://apigargoyle.com/GargoyleApi/beta/getHackingItems?itemId=973846*

* URL with multiple request parameters: To give multiple parameters to a request, separate each parameter with ‘&’ like the example given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getHackingItems?getCount=true&order=uid*


### Response Format

Parameter | Description
--------- | -----------
type | Name of API call
results | List of hacking items
message | status of the API call
count | If true, displays the total count of the results with the filters in place. Otherwise, not displayed in the response body

** A sample response is shown on the right side **


# getHackingPosts

To get a list of Hacking Posts on various forums/boards.

**URL:** *http://apigargoyle.com/GargoyleApi/beta/getHackingPosts*
### Request Format
The getHackingPosts API call can be refined by adding one or more of the following parameters.

Parameter | Description
--------- | -----------
start | start record of the results that is to be retrieved. Default is 0 when start is not set. Allows “=” behavior
limit | Number of records to be retrieved. Default is 10 when limit not set. Maximum limit is 10000. When more data having index > 10000 is to be retrieved set start=10000 and limit = "some amount of results you want"
topicsName | name of the topics; allows “Like” behavior, so any searched pattern contained w/in topicsName will return records
boardsName | Name of the forum/board; allows “Like” behavior, so any searched pattern contained w/in boardsName will return records
postsId | Id of the post. Allows “=” behavior
language | language of the product listing; behavior is “=” to match exact language (list of valid languages below, CASE sensitive, some languages return 0 records). Multiple language names can be given with '\|' as the separator. Languages can be Arabic, Chinese, English, French, German, Italian, Japanese, Mandarin, Persian, Polish, Portuguese, Russian, Swedish, Vietnamese
postMs | ms number in any post; allows “Like” behavior, so any searched pattern contained w/in postMs will return records
postCve | cve number in any post; allows “Like” behavior, so any searched pattern contained w/in postCve will return records
uid | user id of the user. Allows “=” behavior
forumsId | Id of the forum. Allows “=” behavior
order | sorts the records according to the parameter in descending order. The default order parameter is recorded_date
postContent | Content in the post; allows “Like” behavior, so any searched pattern contained w/in postContent will return records
pastDay |
getCount | if set to true, it will return the total number of results with the filters in place.
from | Date (YYYY-MM-DD) from which information was scraped; if “to” is not specified, then information through the present is returned
to | Date (YYYY-MM-DD) to which information was scraped; if “from” is not specified, then information starting from the earliest available in the dB is returned

```http
GET /getHackingPosts HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getHackingPosts",
  "results": [
    {
      "autoTranslated": true,
      "recorded_Time": "05:31:00",
      "softwareTags": null,
      "postedDate": "2014-11-03",
      "uid": 116252,
      "boardsName": null,
      "forumsId": 71,
      "topicsName": "كيف اصبح هاكر .. how to become a hacker ..",
      "postContent": "My love benm your speech is true point by point .. also no harm from public research and take the idea of ​​other topics related to technology etc .. Original theme from here: منتديات القرصان http://www.alkrsan.net/forum/showthread.php?t IMG] code is On HTML code is Off Forum Rules Forum Jump User Control Panel Private Messages Subscriptions Who&#39;s Online Search Forums Forums Home .. ~",
      "postsId": 18104281,
      "postedTime": "05:31:00",
      "language": "Arabic",
      "topicId": 148337,
      "scrapedDate": "2017-04-10",
      "postMs": null,
      "postCve": null,
      "recordedDate": "2014-11-03",
      "recordedTime": "05:31:00",
      "financialTags": null,
      "entity": null,
      "tags": null,
      "originalText": { “OriginalContent”:"حبيبي benm كلامك صحيح نقطة بنقطة .. ايضا لا ضير من البحوث العامة واخذ فكرة بخصوص مواضيع ااخرى تتعلق بالتقنية الخ ----الموضوع الأصلى من هنا: منتديات القرصان http://www.alkrsan.net/forum/showthread.php?t=126095اهلا علي ان شاء الله الفائدة لللجمسع ..--بلاك  منووررر وردة اي ...  benm معدلها بخصوص العلم (for y)"
      }
    }
  ],
  "message": "SUCCESS"
}

```

* URL with single request parameter: To give a single parameter to a request, specify a parameter with its value like examples given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getHackingPosts?postContent=world*

2. *http://apigargoyle.com/GargoyleApi/beta/getHackingPosts?postsId=34299321*

* URL with multiple request parameters: To give multiple parameters to a request, separate each parameter with ‘&’ like the example given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getHackingPosts?getCount=true&order=uid*

### Response Format

Parameter | Description
--------- | -----------
type | Name of API call
results | List of hacking items
message | status of the API call
count | If true, displays the total count of the results with the filters in place. Otherwise, not displayed in the response body

**Example Response:**

A sample response is shown on the right side.


# getHackingThreads

To get a list of Hacking Threads for a forum.

**URL:** *http://apigargoyle.com/GargoyleApi/beta/getHackingThreads*
### Request Format
The getHackingThreads API call can be refined by adding one or more of the following parameters.

Parameter | Description
--------- | -----------
start | start record of the results that is to be retrieved. Default is 0 when start is not set. Allows “=” behavior
limit | Number of records to be retrieved. Default is 10 when limit not set. Maximum limit is 10000. When more data having index > 10000 is to be retrieved set start=10000 and limit = "some amount of results you want"
topicId | Id of the topic. Allows “=” behavior
topicsName | name of the topics; allows “Like” behavior, so any searched pattern contained w/in topicsName will return records
boardsName | Name of the forum/board; allows “Like” behavior, so any searched pattern contained w/in boardsName will return records
postsId | Id of the post. Allows “=” behavior
language | language of the product listing; behavior is “=” to match exact language (list of valid languages below, CASE sensitive, some languages return 0 records). Multiple language names can be given with '\|' as the separator. Languages can be Arabic, Chinese, English, French, German, Italian, Japanese, Mandarin, Persian, Polish, Portuguese, Russian, Swedish, Vietnamese
postMs | ms number in any post; allows “Like” behavior, so any searched pattern contained w/in postMs will return records
postCve | cve number in any post; allows “Like” behavior, so any searched pattern contained w/in postCve will return records
uid | user id of the user. Allows “=” behavior
forumsId | Id of the forum. Allows “=” behavior
order | sorts the records according to the parameter in descending order. The default order parameter is recorded_date
postContent | Content in the post; allows “Like” behavior, so any searched pattern contained w/in postContent will return records
pastDay |
getCount | if set to true, it will return the total number of results with the filters in place.
from | Date (YYYY-MM-DD) from which information was scraped; if “to” is not specified, then information through the present is returned
to | Date (YYYY-MM-DD) to which information was scraped; if “from” is not specified, then information starting from the earliest available in the dB is returned

```http
GET /getHackingThreads HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getHackingThreads",
  "results": {
    "777656": {
      "forumsId": 72,
      "boardsName": ":: hacker  منظمة قانون الهكر organization::",
      "topicsName": "[نقاش] هام بخصوص مشكلة هاك مود ومحاولات حلها..",
      "postCount": 1,
      "posts": [
        {
          "softwareTags": null,
          "postContent": "موضوع جميل شكرا لصاحب الموضوع لتقديم يد العون للأعضاءراجيا من بقية الاعضاء عدم الخروج عن نطاق الموضوعوشكرا مرة اخرى",
          "btcAddress": null,
          "language": "Arabic",
          "postedDate": "None",
          "tags": null,
          "postMs": null,
          "financialTags": null,
          "usersId": "1",
          "pgpKey": null,
          "postCve": null,
          "translatedContent": null,
          "scrapedDate": "2017-05-30",
          "recordedTime": "None",
          "entity": null
        }
      ]
    }
  },
  "message": "SUCCESS"
}

```

* URL with single request parameter: To give a single parameter to a request, specify a parameter with its value like examples given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getHackingThreads?postContent=amazon*

2. *http://apigargoyle.com/GargoyleApi/beta/getHackingThreads?uid=1*

* URL with multiple request parameters: To give multiple parameters to a request, separate each parameter with ‘&’ like the example given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getHackingThreads?getCount=true&order=uid*

### Response Format

Parameter | Description
--------- | -----------
type | Name of API call
results | List of hacking items
message | status of the API call
count | If true, displays the total count of the results with the filters in place. Otherwise, not displayed in the response body

**Example Response:**

A sample response is shown on the right side.
